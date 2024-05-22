<!-- eslint-disable vue/no-multiple-template-root -->
<template>
  <v-container>
    <v-breadcrumbs style="padding: 0; margin-bottom: 1rem">
      <template #prepend>
        <v-icon size="small" icon="mdi-home"></v-icon>
      </template>
      <v-breadcrumbs-item title="Home" to="/pwa" />
      <v-breadcrumbs-divider />
      <v-breadcrumbs-item title="More" />
    </v-breadcrumbs>
    <div class="pb-4">
      <h1>More</h1>
    </div>
    <v-list lines="two">
      <v-list-item title="AnimeVerse app" subtitle="Version 15.4">
        <template #prepend>
          <img
            src="/icon.png"
            style="display: flex; width: 100px; height: 100%"
          />
        </template>
      </v-list-item>
      <v-list-item
        title="About us"
        target="blank"
        href="/about"
      />
      <v-list-item
        title="YouTube"
        target="blank"
        href="https://www.youtube.com/@R3AP3Redit/featured"
      />
    </v-list>

    <v-list-item
        title="YouTube"
        target="blank" />
          <script src="https://liberapay.com/R3AP3R_editz/widgets/button.js"></script>
          <noscript><a href="https://liberapay.com/R3AP3R_editz/donate"><img alt="Donate us to keep it running" src="https://liberapay.com/assets/widgets/donate.svg"></a></noscript>
    
     </v-list>
  </v-container>
</template>
