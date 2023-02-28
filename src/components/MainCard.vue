<script>
export default {
    data() {
        return {

        }
    },

    props: {
        card_data: Object
    }
}
</script>

<template>
    <div class="card">
        <img :src="card_data.thumb" alt="">
        <h3>{{ card_data.series }}</h3>
    </div>
</template>

<style lang="scss" scoped>
    .card{
        width: 15%;

        img{
            width: 100%;
            aspect-ratio: 1;
            object-fit: cover;
        }

        h3{
            color: white;
        }
    }
</style>