<template>
  <div>
    <!-- Your existing template code here -->

    <!-- Continue Watching Section -->
    <div v-if="watchHistory.length > 0">
      <h2>Continue Watching</h2>
      <div v-for="(anime, index) in watchHistory" :key="anime.id">
        <p>{{ anime.title }} - Episode {{ anime.episode }}</p>
        <button @click="resumeAnime(anime)">Resume</button>
      </div>
    </div>
  </div>
</template>

<script setup>
import { useStorage } from "@vueuse/core";
import { ref, watch } from 'vue';

const MAX_WATCH_HISTORY = 6; // Maximum number of anime to save in "Continue Watching"

const watchHistory = useStorage("site-watch", []); // Array to store watched anime

// Function to add a new anime to the watch history
const addToWatchHistory = (anime) => {
  const index = watchHistory.value.findIndex(item => item.id === anime.id);
  if (index !== -1) {
    watchHistory.value.splice(index, 1); // Remove existing entry to move it to the top
  }
  watchHistory.value.unshift(anime); // Add the new anime to the beginning of the array
  if (watchHistory.value.length > MAX_WATCH_HISTORY) {
    watchHistory.value.pop(); // Remove the oldest entry if the array exceeds the maximum limit
  }
};

// Watch for changes in watch history and update the storage
watch(() => watchHistory.value, () => {
  watchHistory.value = watchHistory.value.slice(0, MAX_WATCH_HISTORY); // Ensure the array doesn't exceed the maximum limit
});

// Example function to simulate resuming an anime
const resumeAnime = (anime) => {
  console.log(`Resuming anime: ${anime.title} - Episode ${anime.episode}`);
};
</script>
