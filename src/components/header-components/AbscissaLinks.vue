<script>
export default {
    name: 'AbscissaLinks',
    data: () => ({}),
    props: {
        links: Array
    }

};
</script>

<template>
    <nav id="menu">
        <ul>
            <li v-for="(link, i) in links" :key="i">
                <a :href="link.url" :class="{ 'active': link.current }">{{ link.text.toUpperCase() }}</a>
            </li>
        </ul>
    </nav>
</template>


<style lang="scss" scoped>
#menu {
    ul {
        display: flex;
        gap: 15px;
        font-size: 14px;
        font-weight: 600;

        .active {
            color: dodgerblue;
            border-bottom: 5px solid dodgerblue;
            padding-bottom: 35px;
        }
    }
}
</style>