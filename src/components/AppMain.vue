<script>
export default {
    data() {
        return {

        }
    },

    promps:{
        cards: Array
    }
}
</script>

<template>
    <section>
        <div class="container">
            <div class="card"
                v-for="card in cards" :key="card.series">
                <img :src="card.thumb" alt="">
                
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped> 
    section{
        height: 400px;
        background-color: aquamarine;

        .card{
            width: 15%; 
            height: 100px;
        }
    }
</style>