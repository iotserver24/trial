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
      <v-list-item title="About us" target="blank" href="/about" />
      <v-list-item
        title="YouTube"
        target="blank"
        href="https://youtube.com/@neko_729?si=MpB3qtRB3A_AkgAU"
      />

     <v-list-item
        title="InstaGram"
        target="blank"
        href="https://www.instagram.com/kurumi__002?igsh=Y3BnejNiaHRsbjFh"
      />
<h5> built by: </h5>

<v-list-item
        title="R3AP3R editz"
        target="blank"
        href="https://youtube.com/@r3ap3redit?si=Vl78a8yIioBMj1Dz"
      />

    </v-list>
  </v-container>
</template>
