<script>
import MainCard from "./MainCard.vue"

export default {
    data() {
        return {

        }
    },

    components: {
        MainCard
    },

    props:{
        cards: Array
    }
}
</script>

<template>
    <section>
        <div class="container">
            <div class="current-series">
                CURRENT SERIES
            </div>
            <ul>
                <MainCard 
                  v-for="card in cards" :card_data="card"/>
            </ul>
            <div class="btn">LOAD MORE</div>
        </div>
    </section>
</template>

<style lang="scss" scoped> 
    section{
        padding-bottom: 5rem;
        background-color: #1C1C1C;
        position: relative;

        ul{
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            padding-top: 5rem;
        }

        .btn{
        max-width: 170px;
        padding: 10px 30px;
        border: 1px solid #0282F9;
        color: white;
        cursor: pointer;
        position: absolute;
        bottom: 0;
        margin-bottom: 10px;
        left: 50%;
        transform: translateX(-50%);

        &:hover{
            background-color: #0282F9;
            color: white;
        }

    }
    .current-series{
        position: absolute;
        top: 0;
        transform: translateY(-50%);
        background-color: #0282F9;
        color: white;
        padding: 15px 30px;
        font-weight: bold;
        font-size: 1.3rem;
    }
    }
</style>