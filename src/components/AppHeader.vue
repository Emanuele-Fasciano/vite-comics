<script>
export default{
    data(){
        return{
            headerLinks:[
                {
                    label: "CHARACTERS",
                    link: "#",
                    active: false
                },
                {
                    label: "COMICS",
                    link: "#",
                    active: false
                },
                {
                    label: "MOVIES",
                    link: "#",
                    active: false
                },
                {
                    label: "TV",
                    link: "#",
                    active: false
                },
                {
                    label: "GAMES",
                    link: "#",
                    active: false
                },
                {
                    label: "COLLECTIBLES",
                    link: "#",
                    active: false
                },
                {
                    label: "VIDEOS",
                    link: "#",
                    active: false
                },
                {
                    label: "FANS",
                    link: "#",
                    active: false
                },
                {
                    label: "NEWS",
                    link: "#",
                    active: false
                },
                {
                    label: "SHOP",
                    link: "#",
                    active: false
                },
            ]
        }
    }
}
</script>

<template>
 <header class="container">
    <img src="../assets/dc-logo.png" alt="">
    <ul>
        <li v-for="link in headerLinks" :key="headerLinks.label"
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