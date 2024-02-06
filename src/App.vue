<script>
import { menuItems } from './assets/data/data.js';
import { navbarLinks } from './assets/data/data.js';
import { comics } from './assets/data/dc-comics.js';

import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  name: 'App',
  components: { AppHeader, AppMain, AppFooter },
  data() {
    return {
      menuItems: menuItems,
      navbarLinks: navbarLinks,
      comicsItems: comics
    };
  }
};
</script>


<template>
  <AppHeader class="container" :links="menuItems" />
  <AppMain :comics="comicsItems" />
  <AppFooter :navLinks="navbarLinks" />
</template>


<style lang="scss">
@use './assets/scss/style.scss';
</style>