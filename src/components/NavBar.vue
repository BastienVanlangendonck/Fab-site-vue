<template>
  <header :class="{ 'scrolled-nav': scrolledNav }">
    <nav>
      <div class="branding">
        <router-link to="/"
          ><img src="../assets/logo-250.png" alt="Logo"
        /></router-link>
      </div>
      <ul v-show="!mobile" class="navigation">
        <li><router-link class="link" to="/Massages">Massages</router-link></li>
        <li>
          <router-link class="link" to="/SoinsMagnetisme"
            >Soins energetiques-Manetisme</router-link
          >
        </li>
        <li><router-link class="link" to="/Tarifs">Tarifs</router-link></li>
        <li><router-link class="link" to="/Contact">Contact</router-link></li>
      </ul>
      <div class="icon">
        <i
          @click="toggleMobileNav"
          v-show="mobile"
          class="far fa-bars"
          :class="{ 'icon-active': mobileNav }"
        ></i>
      </div>
      <transition name="mobile-nav">
        <ul v-show="mobileNav" class="dropdown-nav">
          <li @click="toggleMobileNav">
            <router-link class="link" to="/">Accueil</router-link>
          </li>
          <li @click="toggleMobileNav">
            <router-link class="link" to="/Massages">Massages</router-link>
          </li>
          <li @click="toggleMobileNav">
            <router-link class="link" to="/SoinsMagnetisme"
              >Soins energetiques-Manetisme</router-link
            >
          </li>
          <li @click="toggleMobileNav">
            <router-link class="link" to="/Tarifs">Tarifs</router-link>
          </li>
          <li @click="toggleMobileNav">
            <router-link class="link" to="/Contact">Contact</router-link>
          </li>
        </ul>
      </transition>
    </nav>
  </header>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      scrolledNav: null,
      mobile: null,
      mobileNav: null,
      windowWidth: null,
    };
  },
  created() {
    window.addEventListener("resize", this.checkScreen);
    this.checkScreen();
  },
  mounted() {
    window.addEventListener("scroll", this.updateScroll);
  },
  methods: {
    toggleMobileNav() {
      this.mobileNav = !this.mobileNav;
    },

    updateScroll() {
      const scrollPosition = window.scrollY;
      if (scrollPosition > 50) {
        this.scrolledNav = true;
        return;
      }
      this.scrolledNav = false;
    },

    checkScreen() {
      this.windowWidth = window.innerWidth;
      if (this.windowWidth <= 750) {
        this.mobile = true;
        return;
      }
      this.mobile = false;
      this.mobileNav = false;
      return;
    },
  },
};
</script>

<style scoped>
header {
  background: rgb(44, 21, 76);
  background: linear-gradient(
    90deg,
    rgba(44, 21, 76, 1) 65%,
    rgba(113, 73, 151, 1) 100%
  );
  z-index: 99;
  width: 100%;
  position: fixed;
  transition: 0.5s ease all;
  top: 0;
}

nav {
  position: relative;
  display: flex;
  flex-direction: row;
  padding: 12px 0;
  transition: 0.5s ease all;
  width: 90%;
  margin: 0 auto;
}

ul,
.link {
  font-weight: 500;
  color: white;
  list-style: none;
  text-decoration: none;
}

li {
  text-transform: uppercase;
  padding: 16px;
  margin-left: 16px;
  margin-left: 0;
}

.link {
  font-size: 14px;
  transition: 0.5s ease all;
  padding-bottom: 4px;
  border-bottom: 2px solid transparent;
}

.link:hover {
  font-size: 1.1rem;
  border-color: rgba(255, 255, 255, 0.507);
}

.branding {
  display: flex;
  align-items: center;
}

img {
  width: 50px;
  transition: 0.5s ease all;
}

.navigation {
  display: flex;
  align-items: center;
  flex: 1;
  justify-content: flex-end;
}

.icon {
  display: flex;
  align-items: center;
  position: absolute;
  top: 0;
  right: 24px;
  height: 100%;
}

i {
  cursor: pointer;
  font-size: 24px;
  transition: 0.8s ease all;
}

.icon-active {
  transform: rotate(180deg);
}

.dropdown-nav {
  display: flex;
  flex-direction: column;
  position: fixed;
  width: 100%;
  max-width: 250px;
  height: 100%;
  background-color: rgb(61, 18, 58);
  top: -16px;
  left: -16px;
}

.mobile-nav-enter-active,
.mobile-nav-leave-active {
  transition: 1s ease all;
}

.mobile-nav-enter-from,
.mobile-nav-leave-to {
  transform: translateX(-275px);
}

.mobile-nav-enter-to {
  transform: translateX(0);
}

.scrolled-nav {
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1),
    0 2px 4px -1px rgba(0, 0, 0, 0.06);
}

.scrolled-nav > nav {
  padding: 8px 0;
}

.scrolled-nav > nav > .branding > img {
  width: 40px;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1),
    0 2px 4px -1px rgba(0, 0, 0, 0.06);
}

@media (min-width: 1140px) {
  nav {
    max-width: 1140px;
  }
}
/* 
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
} */
</style>
