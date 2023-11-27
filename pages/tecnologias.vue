<template>
    <v-window
    v-model="onboarding"
    show-arrows
    direction="vertical"
  >
  <tecnologias-slide1 />
  <tecnologias-slide2 />
  <tecnologias-slide3 />
  </v-window>
</template>

<!-- !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! -->

<style>

</style>

<!-- !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! -->

<script>
  export default {
    data: () => ({
      length: 3,
      onboarding: 0,
    }),
  }
</script>