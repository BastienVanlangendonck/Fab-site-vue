<template>
  <div id="nav">
    <NavBar />
    <!--     <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> -->
  </div>
  <router-view />
</template>
<script>
import NavBar from "@/components/NavBar.vue";

export default {
  components: {
    NavBar,
  },
};
</script>

<style>
@font-face {
  font-family: "Merienda";
  src: local("Merienda"),
    url(/fonts/Merienda/Merienda-Regular.ttf) format("truetype");
}

body {
  margin: auto;
  height: 100vh;
  background: rgb(229, 217, 232);
  background: radial-gradient(
    circle,
    rgba(229, 217, 232, 1) 0%,
    rgba(166, 117, 177, 1) 40%
  );
}
a {
  text-decoration: none;
}
#app {
  font-family: Merienda;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: white;
}

#nav a {
  color: white;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
