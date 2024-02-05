<script>
import HeaderLinks from './HeaderLinks.vue'

export default {
    name: 'AppHeader',
    data: () => ({}),
    components: { HeaderLinks },
    props: {
        links: Array
    }
};
</script>

<template>
    <header>
        <div id="logo-header">
            <img src="@/assets/img/dc-logo.png" alt="DC Logo">
        </div>
        <HeaderLinks :links="links" />
    </header>
</template>




<style scoped>
header {
    height: 100px;
    display: flex;
    flex-shrink: 0;
    justify-content: space-between;
    align-items: center;
    padding: 0 150px;
}

#logo-header img {
    max-width: 80px;
    margin-top: 10px;
}
</style>