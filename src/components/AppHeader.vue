<script>
import HorizontalLinks from './header_components/HorizontalLinks.vue'
import LogoSm from './header_components/LogoSm.vue'

export default {
    name: 'AppHeader',
    data: () => ({}),
    components: { HorizontalLinks, LogoSm, },
    props: {
        links: Array
    }
};
</script>

<template>
    <header>
        <LogoSm />
        <HorizontalLinks :links="links" />
    </header>
</template>




<style scoped>
header {
    height: 100px;
    display: flex;
    flex-shrink: 0;
    justify-content: space-between;
    align-items: center;
    padding: 0 100px;
}
</style>