<script>
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <section>
        <div class="container">
            <p>Content goes here</p>
        </div>

        <!-- <div class="card"
                    v-for="icon in icons">
                    <img :src="'../assets/buy-' + icon.img" alt="">
                    <span>{{ icon.text }}</span>
                </div> -->
    </section>
</template>

<style lang="scss" scoped> 
    section{
        background-color: black;

        p{
            color: white;
            padding: 5rem 0;
        }
    }
</style>