<script>
export default {
    data() {
        return {

        }
    },

    props: {
        icon_data: Object
    }
}
</script>

<template>
    <div class="card">
        <img :src="'../src/assets/buy-' + icon_data.img" alt="">
        <span>{{ icon_data.text }}</span>
    </div>
</template>

<style lang="scss" scoped>
    .card{
        width: 15%;
        padding: 3rem 0;
        display: flex;
        align-items: center;

        img{
            width: 50px;
            margin-right: 20px;
        }
        }
</style>