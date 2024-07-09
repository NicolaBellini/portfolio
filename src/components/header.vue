<script>
export default {
  mounted() {
    gsap.from("header img", { duration: 1.5, opacity: 0, top: 50 });
  },
};
</script>
<template>
  <header>
    <nav>
      <ul>
        <li>home</li>
        <li>
          <img class="logo" src="/public/img/logo1.png" alt="" />
        </li>
        <li>about</li>
      </ul>
    </nav>
  </header>
</template>

<style scoped lang="scss">
@use "../assets/scss/partials/variables" as *;
@use "../assets/scss/main.scss";
header {
  position: fixed;
  width: 100%;
  z-index: 999;
  display: flex;
  justify-content: center;
  padding: 20px 25px;
  background-color: $background-color;
  color: $gray-light;
  overflow: hidden;
  nav {
    width: 70%;
    ul {
      display: flex;
      padding: 0;
      margin: 0;
      justify-content: space-between;

      li {
        list-style: none;
        margin-inline-end: 10px;
        .logo {
          max-width: 110px;
          opacity: 1;
          height: auto;
          position: absolute;
          top: 0px;
          left: 50%;
          color: white;
          transform: translate(-50%, -20%);
        }
      }
    }
  }
}
</style>
