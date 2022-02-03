<template>
  <header class="header">
    <div class="logo">
      <a class="home-link" href="/">
        <img class="header-img" src="../assets/logo-250.png" alt="Logo" />
        <h1 class="header-title">L'âme-agit en soi</h1>
      </a>
    </div>
    <ul class="nav">
      <li class="nav-items">
        <router-link to="/Massages">Massages</router-link>
      </li>
      <li class="nav-items">
        <router-link to="/SoinsMagnetisme">Soins energetiques-Manetisme</router-link>
      </li>
      <li class="nav-items">
        <router-link to="/Tarifs">Tarifs</router-link>
      </li>
      <li class="nav-items">
        <router-link to="/About">A propos</router-link>
      </li>
      <li class="nav-items">
        <router-link to="/Contact">Contact</router-link>
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: "NavBar",
};
</script>

<style scoped>
.header {
  background: rgb(44, 21, 76);
  background: linear-gradient(
    90deg,
    rgba(44, 21, 76, 1) 65%,
    rgba(113, 73, 151, 1) 100%
  );
}
.logo {
  max-height: 6rem;
}
.home-link {
  display: flex;
  text-decoration: none;
}
.header-img {
  width: 6rem;
  height: 6rem;
  margin: 1.5rem;
}
.header-title {
  display: flex;
  align-self: center;
  font-size: 2rem;
  font-style: italic;
  margin: 1.5rem;
  color: white;
}
.nav {
  display: flex;
  list-style-type: none;
  justify-content: end;
  margin-bottom: auto;
}

.nav-items {
  font-weight: bold;
  margin: 0rem 1rem 1rem 1rem;
}
</style>
