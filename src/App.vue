<script>
import headerVue from "./components/header.vue";
import imageDragger from "./components/image-dragger.vue";
import parallaxHero from "./components/parallaxHero.vue";
// import imageDragger from "./components/image-dragger.vue";

export default {
  components: {
    headerVue,
    imageDragger,
    parallaxHero,
  },
};
</script>

<template>
  <headerVue />
  <parallaxHero />
  <imageDragger />
</template>

<style lang="scss" scoped>
@use "./assets/scss/partials/variables" as *;
@use "./assets/scss/main.scss";
h1 {
  color: $gray-dark;
}
</style>
