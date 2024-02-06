<script>
import { comics } from '@/assets/data/dc-comics';

export default {
    name: 'ComicsGrid',
    data: () => ({}),
    props: {
        comics: Array,
    }
};
</script>

<template>
    <div class="row">
        <div class="comic-card" v-for="(comic, index) in comics" :key="index">
            <img :src="comic.thumb" alt="Comic Thumbnail" class="comic-thumb">
        </div>
    </div>
</template>


<style scoped>
.row {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 20px;
}

.comic-card {
    height: 200px;
    width: calc(100% / 6 - 20px);
    margin-bottom: 20px;
    background-color: white;
    border-radius: 8px;

}

.comic-card img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}
</style>