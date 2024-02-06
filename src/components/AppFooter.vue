<script>
import AbscissaNavbar from './footer-components/AbscissaNavbar.vue';
import FooterJumbotron from './footer-components/FooterJumbotron.vue';

export default {
    name: 'AppFooter',
    data: () => ({}),
    components: { AbscissaNavbar, FooterJumbotron },
    props: {
        navLinks: Array
    }
};
</script>

<template>
    <footer>
        <AbscissaNavbar :links="navLinks" />
        <FooterJumbotron />
    </footer>
</template>


<style scoped>
footer {
    height: 120px;
    background-color: dodgerblue;
}
</style>