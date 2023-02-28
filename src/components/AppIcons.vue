<script>
import SingleIcon from "./SingleIcon.vue"

export default {
    data() {
        return {
            
        }
    },

    components: {
        SingleIcon
    },

    props: {
        icons: Array
    }
}
</script>

<template>
    <section>
        <div class="container">
            <SingleIcon v-for="icon in icons" :icon_data = icon />
        </div>
        
    </section>
</template>

<style lang="scss" scoped>
    section{
        background-color:#0282F9;
        color: white;

        .container{
            display: flex;
            justify-content: space-between;
            
        }

    }
</style>