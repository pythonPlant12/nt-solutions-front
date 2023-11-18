<script>
export default {
  data() {
    return {
      slides: [
        {
        src: "https://github.com/pythonPlant12/vuetify/blob/main/assets/css/videos/carousel-1.mp4",
      }
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
      <v-carousel-item v-for="(slide, i) in slides" :key="i">
        <video width="100%" height="100%" controls>
          <source :src="slide.src" type="video/mp4">
          Your browser does not support the video tag.
        </video>
      </v-carousel-item>
    </v-carousel>
  </div>
</template>

<style>
</style>
