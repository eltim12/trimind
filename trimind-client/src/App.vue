<template>
  <v-app>
    <v-main>
      <NavigationBar />
      <router-view />
      <TrimindFooter />
    </v-main>
  </v-app>
</template>

<script setup>
//
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap");
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@100..900&family=Space+Mono:ital,wght@0,400;0,700;1,400;1,700&display=swap");

#app {
  font-family: "Inter", sans-serif;
  // position: absolute;
  inset: 0;
  display: flex;
  place-content: center;
  align-items: center;
  overflow: hidden;

  .text-mono {
    font-family: "Space Mono", monospace !important;
  }
}

/* This is just to transition when you change the viewport size. */
* {
  transition: all 0.5s ease-out;
}


</style>
