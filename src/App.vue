<script>
import { menuItems } from '@/assets/data/data.js';

import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';



export default {
  name: 'App',
  components: { AppHeader, AppMain, AppFooter },
  data() {
    return {
      menuItems: menuItems,
    };
  },
};
</script>


<template>
  <AppHeader :links="menuItems" />
  <AppMain />
  <AppFooter />
</template>


<style lang="scss">
@use './assets/scss/style.scss';
</style>