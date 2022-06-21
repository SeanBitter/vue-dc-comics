<template>
<div class="section">
    <div class="container">
        <div class="d-flex justify-content-between">
            <div class="btn-section">
                <button class="sign-up-btn fw-bold">SIGN-UP NOW!</button>
            </div>
            <div class="social-section d-flex">
                <ul class="list-unstyled d-flex align-items-center">
                    <li class="text-primary fw-bold follow-us">FOLLOW US</li>
                    <li v-for="(social, i) in socialNetworks" :key="i">
                        <a :href="social.href"><img :src="'/img/footer-' + social.name + '.png'" :alt="'DC' + social.name"></a>
                    </li>

                </ul>
            </div>
        </div>
    </div>
</div>
</template>

<script>
    export default {
        name: 'SignUpBanner',

        data() {
            return {
                socialNetworks: [
                    {
                        name: "facebook",
                        href: "#",
                    },

                    {
                        name: "twitter",
                        href: "#",
                    },

                    {
                        name: "youtube",
                        href: "#",
                    },

                    {
                        name: "pinterest",
                        href: "#",
                    },

                    {
                        name: "periscope",
                        href: "#",
                    },
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
@import "../assets/scss/variables";
    .section {
        background-color: $secondary;
        padding-top: 1.5rem;
        padding-bottom: 0.5rem;
        position: sticky;
        z-index: 2;
        bottom: 0;
        left: 0;
        right: 0;

            .sign-up-btn {
                border: 2px solid $primary;
                background-color: transparent;
                color: white;
                padding: 0.5rem;
                font-family: Arial, Helvetica, sans-serif;
                transition: 0.3s ease-in-out;

                &:hover {
                    background-color: rgb(105, 110, 112);
                    color: rgb(213, 231, 231);
                    transition: 0.3s ease-in-out;
                }
            };

            .follow-us {
                font-size: 1.2rem;
                vertical-align: bottom;
            }

            ul li a {
                padding: 0 0.5rem;
            }
    }
</style>