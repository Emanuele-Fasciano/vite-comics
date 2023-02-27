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
            <div class="card">
                <img src="../assets/buy-comics-digital-comics.png" alt="">
                <span>DIGITAL COMICS</span>
            </div>
            <div class="card">
                    <img src="../assets/buy-comics-digital-comics.png" alt="">
                    <span>DC MERCHANDISE</span>
                </div>
                <div class="card">
                    <img src="../assets/buy-comics-digital-comics.png" alt="">
                    <span>SUBSCRIPTION</span>
                </div>
                <div class="card">
                    <img src="../assets/buy-comics-digital-comics.png" alt="">
                    <span>COMIC SHOP LOCATION</span>
                </div>
                <div class="card">
                    <img src="../assets/buy-comics-digital-comics.png" alt="">
                    <span>DC POWER VISA</span>
                </div>
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
        }

    }
</style>