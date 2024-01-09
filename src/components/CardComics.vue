<script>
export default {
    name: 'CardComics',
    props: {
        comic: Object
    }
}
</script>
<template lang="">
    <div class="card">
        <img :src="comic.thumb" :alt="comic.series">
        <h4>{{comic.series}}</h4>
    </div>
</template>
<style lang="scss" scoped>
.card {
    width: calc(100% / 6 - 30px);
    margin: 15px;


    img {
        width: 100%;
        height: 60%;
    }

    h4 {
        color: white;
        text-transform: uppercase;
        margin-top: 10px;
    }
}
</style>