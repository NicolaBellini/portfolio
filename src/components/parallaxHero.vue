<script>
export default {};
</script>

<template>
  <div class="hero">
    <div class="d-flex justify-content-between name">
      <h1>Nicola</h1>
      <p>Web Devoleper</p>
    </div>
    <div class="d-flex justify-content-between surname">
      <p>Creative soul</p>
      <h1>Bellini</h1>
    </div>
    <div></div>
    <div></div>
  </div>
</template>

<style scoped lang="scss">
.hero {
  height: 100vh;
  padding: 0 5%;
  background-color: black;
  color: white;
  h1 {
    font-size: 10rem;
  }
  .name,
  .surname {
    height: 50%;
    border-bottom: 1px solid white;
  }
}
</style>
