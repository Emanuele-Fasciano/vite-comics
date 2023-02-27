<script>
export default {
    data() {
        return {
            dcComicsLinks:[
                {
                    label: "Characters",
                    link: "#"
                },
                {
                    label: "Comics",
                    link: "#"
                },
                {
                    label: "Movies",
                    link: "#"
                },
                {
                    label: "TV",
                    link: "#"
                },
                {
                    label: "Games",
                    link: "#"
                },
                {
                    label: "Videos",
                    link: "#"
                },
                {
                    label: "News",
                    link: "#"
                },
            ],

            shopLinks: [
                {
                    label: "Shop DC",
                    link: "#"
                },
                {
                    label: "Shop DC Collectibles",
                    link: "#"
                },
            ],

            dcLinks: [
                {
                    label: "Term Of Use",
                    link: "#"
                },
                {
                    label: "Privacy Policy(New)",
                    link: "#"
                },
                {
                    label: "Ad Choices",
                    link: "#"
                },
                {
                    label: "Advertising",
                    link: "#"
                },
                {
                    label: "Jobs",
                    link: "#"
                },
                {
                    label: "Subscriptions",
                    link: "#"
                },
                {
                    label: "Talent Workshops",
                    link: "#"
                },
                {
                    label: "CPSC Certificates",
                    link: "#"
                },
                {
                    label: "Ratings",
                    link: "#"
                },
                {
                    label: "Shop Hepl",
                    link: "#"
                },
                {
                    label: "Contact Us",
                    link: "#"
                }
            ],

            sitesLinks: [
                {
                    label: "DC",
                    link: "#"
                },
                {
                    label: "MAD Magazine",
                    link: "#"
                },
                {
                    label: "DC Kids",
                    link: "#"
                },
                {
                    label: "TV",
                    link: "#"
                },
                {
                    label: "DC Universe",
                    link: "#"
                },
                {
                    label: "DC Power Visa",
                    link: "#"
                },
            ],
            

        }
    }
}
</script>

<template>
    <footer>
        <div class="container d-flex">
            <div class="links-col d-flex">
                <div class="comics-link">
                    <h3>DC COMICS</h3>
                    <ul>
                        <li v-for="link in dcComicsLinks" :key="link.label">
                            {{ link.label }}
                        </li>
                    </ul>

                    <h3>SHOP</h3>
                    <ul>
                        <li v-for="link in shopLinks" :key="link.label">
                                {{ link.label }}
                        </li>
                    </ul>  
                </div>

                <div class="dc-links">
                    <h3>DC</h3>
                    <ul>
                        <li v-for="link in dcLinks" :key="link.label">
                                {{ link.label }}
                        </li>
                    </ul>
                </div>

                <div class="sites-links">
                        <h3>SITES</h3>
                            <ul>
                                <li v-for="link in sitesLinks" :key="link.label">
                                    {{ link.label }}
                            </li>
                            </ul>
                    </div>
            </div>
            <div class="img-col">
                <img src="../assets/dc-logo-bg.png" alt="">
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
footer{
    background-image: url(/footer-bg.jpg);
    color: white;
}

.links-col{
    width: 50%;
    gap: 40px;
    padding: 3rem 0;

    h3{
        margin: 1rem 0;
    }

    li{
        margin: 7px 0;
        color: hsl(0deg 0% 47%);

        &:hover{
            color: white
        };
    }
}

img{
    width: 77%;
}
</style>