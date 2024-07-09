<template>
  <div class="hero">
    <div class="hero-bg"></div>
    <div class="hero-content">
      <h1>Benvenuti nel nostro sito</h1>
      <p>Scopri di più sulla nostra missione e sui nostri valori.</p>
    </div>
  </div>
</template>

<script>
// import { gsap } from "gsap";

export default {
  mounted() {
    window.addEventListener("scroll", this.handleScroll);
  },
  beforeDestroy() {
    window.removeEventListener("scroll", this.handleScroll);
  },
  methods: {
    handleScroll() {
      const scrollPosition = window.scrollY;
      gsap.to(".hero-bg", {
        y: scrollPosition * 0.6,
        ease: "power2.out",
        duration: 1200,
        // fill: "forwards",
      });
    },
  },
};
</script>

<style scoped lang="scss">
.hero {
  position: relative;
  height: 100vh;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  color: white;
  background: linear-gradient(to top, rgba(0, 0, 0, 1), rgba(0, 0, 0, 0));

  .hero-bg {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: url("/img/vasilina-sirotina-EFHbtvK_Cb4-unsplash.jpg")
      center/cover no-repeat;
    z-index: -1;
  }

  .hero-content {
    position: relative;
    z-index: 1;
  }

  h1 {
    font-size: 3rem;
    margin: 0;
  }

  p {
    font-size: 1.25rem;
  }
}
</style>
