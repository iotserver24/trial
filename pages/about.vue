<script setup>
useSeoMeta({
  ogTitle: "About",
  ogDescription: "About AnimeVerse...",
  ogImage: "logo.png",
  ogUrl: "[og:url]",
  twitterTitle: "About",
  twitterDescription: "About AnimeVerse...",
  twitterImage: "logo.png",
  twitterCard: "summary",
});

useHead({
  htmlAttrs: {
    lang: "en",
  },
  title: "About",
});
</script>
<template>
  <v-container>
    <div style="height: fit-content; display: grid; place-items: center">
      <div class="pa-5" style="background-color: #212121">
        <h1><img src="/logo.png" alt="loho" height="50" /></h1>
        <p>
          AnimeVerse is an anime streaming platform that offer free
          anime with no ADs and install it as Android or IOS web app. <br />
          Build with Nuxt 3, Vuetify and AnimeVerse's V2 API.
        </p>
       
        
        <!-- <script src="https://liberapay.com/R3AP3R_editz/widgets/button.js"></script>
<noscript><a href="https://liberapay.com/R3AP3R_editz/donate"><img alt="Donate using Liberapay" src="https://liberapay.com/assets/widgets/donate.svg"></a></noscript>
         -->
          
       
        <div class="my-5">
          <h1>Donation</h1>
          We do not use ADs and rely on donation to keep the website running forever. 
          You can consider donating us to keep it alive without ads forever!! <br>
          <v-btn
            class="mt-4"
            color="yellow-darken-1"
            prepend-icon="mdi-cash"
            href="https://liberapay.com/R3AP3R_editz/"
          >
            Donation
          </v-btn>
        </div>
      </div>
    </div>
  </v-container>
</template>
