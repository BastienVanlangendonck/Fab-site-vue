<template>
  <div id="nav">
    <NavBar />
  </div>
  <router-view />
  <div id="footer">
    <Footer />
  </div>
</template>
<script>
import NavBar from "@/components/NavBar.vue";
import Footer from "@/components/Footer.vue";

export default {
  components: {
    NavBar,
    Footer,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Merienda:wght@400;700&display=swap");

body {
  margin: auto;
  height: 100%;
  background-image: url("./assets/fdv.png");
  background-color: #724997;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
#app {
  font-family: Merienda;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: white;
}
</style>
