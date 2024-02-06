<script>
import AbscissaNavbar from './footer-components/AbscissaNavbar.vue';


export default {
    name: 'AppFooter',
    data: () => ({}),
    components: { AbscissaNavbar, },
    props: {
        navLinks: Array
    }
};
</script>

<template>
    <footer>
        <AbscissaNavbar :links="navLinks" />
    </footer>
</template>


<style scoped>
footer {
    height: 120px;
    background-color: dodgerblue;
}
</style>