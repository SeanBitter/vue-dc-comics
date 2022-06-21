<template>
    <div class="section">
        <div class="container">
            <div class="row justify-content-md-center">
                <div class="col-sm-4 col-md-3 col-lg-2 d-flex align-items-center" v-for="(icon, i) in blueBannerIcon" :key="i">
                    <div class="py-2 icon-name">
                        <a href="#"><img :src="'/img/' + icon.img" :alt="icon.name" width="40"></a>
                    </div>
                    <div class="ps-3">{{ icon.name }}</div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
        name: 'BlueBanner',

        data() {
            return {
                blueBannerIcon: [
                    {
                        name: "DIGITAL COMICS",
                        img: "buy-comics-digital-comics.png",
                    },

                    {
                        name: "DC MERCHANDISE",
                        img: "buy-comics-merchandise.png",
                    },

                    {
                        name: "SUBSCRIPTION",
                        img: "buy-comics-subscriptions.png",
                    },

                    {
                        name: "COMIC SHOP LOCATOR",
                        img: "buy-comics-shop-locator.png",
                    },

                    {
                        name: "DC POWER VISA",
                        img: "buy-dc-power-visa.svg",
                    },
                ],
            }
        }
    }
</script>

<style lang="scss" scoped>
@import "../assets/scss/variables";

    .section {
        background-color: $primary;
        padding: 2rem 0;
        font-family: Arial, Helvetica, sans-serif;

        .icon-name {
            transition: 0.3s ease-in;

            &:hover {
                transform: scale(1.2);
                transition: 0.3s ease-in;
            }
        }
    }
</style>