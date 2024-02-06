<script>
export default {
    name: 'AbscissaNavbar',
    data: () => ({}),
    props: {
        links: Array
    }
};
</script>

<template>
    <nav class="container">
        <ul>
            <li v-for="(link, i) in links" :key="i">
                <a href="#">
                    <img :src="link.imagePath" :alt="link.text">
                    <span>{{ link.text.toUpperCase() }}</span>
                </a>
            </li>
        </ul>
    </nav>
</template>


<style scoped lang="scss">
nav {
    position: relative;
    display: flex;
    flex-shrink: 0;
    justify-content: center;
    padding: 20px 0;

    ul {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 30px;

        a {
            display: flex;
            align-items: center;
            color: white;
            font-size: 14px;
            gap: 20px;
            white-space: nowrap;

            img {
                max-width: 50px;
            }
        }
    }
}
</style>