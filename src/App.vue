<script>
import { menuItems } from '@/assets/data/data.js';
import { navbarLinks } from './assets/data/data.js';

import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';



export default {
  name: 'App',
  components: { AppHeader, AppMain, AppFooter },
  data: () => ({
    menuItems: menuItems,
    navbarLinks: navbarLinks,
  }),
};
</script>


<template>
  <AppHeader class="container" :links="menuItems" />
  <AppMain />
  <AppFooter :navLinks="navbarLinks" />
</template>


<style lang="scss">
@use './assets/scss/style.scss';
</style>