<script>
import ComicsGrid from './main-components/ComicsGrid.vue';

export default {
    name: 'AppMain',
    data: () => ({}),
    components: { ComicsGrid },
    props: {
        comics: Array
    }
};
</script>

<template>
    <main>
        <ComicsGrid :comics="comics" />
    </main>
</template>


<style scoped>
main {
    min-height: 150px;
    background-color: rgb(28, 28, 28);
    text-align: center;
    line-height: 140px;
    color: white;
}
</style>