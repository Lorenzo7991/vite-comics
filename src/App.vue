<script>
import { menuItems } from '@/assets/data/data.js';

import AppHeader from './components/AppHeader.vue';

export default {
  name: 'App',
  components: { AppHeader, },
  data() {
    return {
      menuItems: menuItems,
    };
  },
};
</script>


<template>
  <AppHeader :links="menuItems" />
</template>


<style lang="scss">
@use './assets/scss/style.scss';
</style>