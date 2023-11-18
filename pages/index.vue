<script>
export default {
  data() {
    return {
      slides: [
        "https://picsum.photos/1200/900",
        "https://picsum.photos/1200/900",
        "/css/videos/carousel-1.mp4",
        "https://picsum.photos/1200/900"
      ],
    };
  },
};
</script>

<template>
  <div class="main-div">
    <v-carousel
      :continuous="true"
      :show-arrows="true"
      hide-delimiter-background
      delimiter-icon="mdi-square"
      height="50rem"
    >
      <v-carousel-item v-for="(slide, i) in slides" :key="i" :src="slide">
      </v-carousel-item>
    </v-carousel>
  </div>
</template>

<style>
</style>
