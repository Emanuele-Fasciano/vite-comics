<script>
export default {
    data() {
        return {
            cards: [
                {
                    img:"comics-digital-comics.png",
                    text:"DIGITAL COMICS"
                },
                {
                    img: "comics-merchandise.png",
                    text: "DC MERCHANDISE"
                },
                {
                    img: "comics-subscriptions.png",
                    text: "SUBSCRIPTION"
                },
                {
                    img: "comics-shop-locator.png",
                    text: "COMIC SHOP LOCATOR"
                },
                {
                    img: "dc-power-visa.svg",
                    text: "DC POWER VISA"
                },
            ]
        }
    }
}
</script>

<template>
    <section>
        <div class="container">
            <div class="card"
                v-for="card in cards">
                <img :src="'../src/assets/buy-' + card.img " alt="">
                <span>{{ card.text }}</span>
            </div>
            <!-- <div class="card">
                    <img src="../assets/buy-comics-merchandise.png" alt="">
                    <span>DC MERCHANDISE</span>
                </div>
                <div class="card">
                    <img src="../assets/buy-comics-subscriptions.png" alt="">
                    <span>SUBSCRIPTION</span>
                </div>
                <div class="card">
                    <img src="../assets/buy-comics-shop-locator.png" alt="">
                    <span>COMIC SHOP LOCATION</span>
                </div>
                <div class="card">
                    <img src="../assets/buy-dc-power-visa.svg" alt="">
                    <span>DC POWER VISA</span>
                </div> -->
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