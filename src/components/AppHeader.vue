<script>
export default{
    data(){
        return{
            
        }
    },

    props: {
        links: Array
    }
}
</script>

<template>
 <header class="container">
    <img src="../assets/dc-logo.png" alt="">
    <ul>
        <li v-for="link in links" :key="links.label"
            @mouseover="link.active = true"
            @mouseleave="link.active = false"
            :class="(link.active == true) ? 'active' : ''">
            {{ link.label }}
        </li>
    </ul>

 </header>
</template>

<style lang="scss" scoped>
    header{
        display: flex;
        justify-content: space-between;

        img{
            padding: 1.5rem 0;
        }

        ul{
            display: flex;
            align-items: center;

            li{
                padding: 0 0.5rem;
                height: 100%;
                line-height: 150px;

            }
            
        }
    }

    .active{
        color: #0282F9;
        box-shadow: 0 7px 2px -2px #0282F9;
        
    }
</style>