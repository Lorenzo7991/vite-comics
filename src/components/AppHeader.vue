<script>
import AbscissaLinks from './header-components/AbscissaLinks.vue'
import LogoSmall from './header-components/LogoSmall.vue'

export default {
    name: 'AppHeader',
    data: () => ({}),
    components: { AbscissaLinks, LogoSmall },
    props: {
        links: Array
    }
};
</script>

<template>
    <header>
        <LogoSmall />
        <AbscissaLinks :links="links" />
    </header>
</template>




<style scoped>
header {
    height: 100px;
    display: flex;
    flex-shrink: 0;
    justify-content: space-between;
    align-items: center;
}
</style>