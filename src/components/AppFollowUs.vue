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
        <div class="container d-flex">
            <span class="btn">SING-UP NOW</span>
            <div class="links d-flex">
                <span>FOLLOW US</span>
                <ul class="d-flex">
                    <li><img src="../assets/footer-facebook.png" alt=""></li>
                    <li><img src="../assets/footer-twitter.png" alt=""></li>
                    <li><img src="../assets/footer-youtube.png" alt=""></li>
                    <li><img src="../assets/footer-pinterest.png" alt=""></li>
                    <li><img src="../assets/footer-periscope.png" alt=""></li>
                </ul>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>

    section{
        background-color: #303030;
    }
    .container{
        justify-content: space-between;
        align-items: center;
    }

    .btn{
        margin: 3rem 0;
        padding: 10px;
        border: 1px solid #0282F9;
        color: white;
        cursor: pointer;

        &:hover{
            background-color: white;
            color: #0282F9;
        }
    }

    .links span{
        line-height: 60px;
        color: #0282F9;
        font-weight: bold
    } 

    li{
        margin: 10px;
    }

    
</style>