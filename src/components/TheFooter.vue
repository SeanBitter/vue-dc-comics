<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-2">
                    <div>
                        <h6>DC COMICS</h6>
                        <ul class="list-unstyled">
                            <li v-for="(link, i) in dcComics" :key="i">
                                <a :href="link.href">{{ link.name }}</a>
                            </li>
                        </ul>
                        <h6>SHOP</h6>
                        <ul class="list-unstyled">
                            <li v-for="(link, i) in shop" :key="i">
                                <a :href="link.href">{{ link.name }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="col-2">
                    <div>
                        <h6>DC</h6>
                        <ul class="list-unstyled">
                            <li v-for="(link, i) in dc" :key="i">
                                <a :href="link.href">{{ link.name }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="col-2">
                    <div>
                        <h6>SITES</h6>
                        <ul class="list-unstyled">
                            <li v-for="(link, i) in sites" :key="i">
                                <a :href="link.href">{{ link.name }}</a>
                            </li>
                        </ul>
                    </div>
                </div>
                <div class="col-6">
                    <div class="d-flex align-items-center position-relative">
                        <img src="/img/dc-logo-bg.png" alt="Logo DC footer" class="logo-footer w-75 position-absolute">
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
    export default {
        name: 'TheFooter',

        data() {
            return {
                dcComics: [
                    {
                        name: "Characters",
                        href: "#",
                    },

                    {
                        name:"Comics",
                        href: "#"
                    },

                    {
                        name: "Movies",
                        href: "#",
                    },

                    {
                        name: "TV",
                        href: "#",
                    },

                    {
                        name: "Games",
                        href: "#",
                    },

                    {
                        name: "Video",
                        href: "#",
                    },

                    {
                        name: "News",
                        href: "#",
                    },
                ],

                shop: [
                    {
                        name: "Shop DC",
                        href: "#",
                    },

                    {
                        name: "Shop DC Collectibies",
                        href: "#",
                    },
                ],

                dc: [
                    {
                        name: "Terms of Use",
                        href: "#",
                    },

                    {
                        name: "Privacy Policy (New)",
                        href: "#",
                    },

                    {
                        name: "Ad Choices",
                        href: "#",
                    },

                    {
                        name: "Advertising",
                        href: "#",
                    },

                    {
                        name: "Jobs",
                        href: "#",
                    },

                    {
                        name: "Subscriptions",
                        href: "#",
                    },

                    {
                        name: "Talent Workshops",
                        href: "#",
                    },

                    {
                        name: "CPSC Certificates",
                        href: "#",
                    },

                    {
                        name: "Ratings",
                        href: "#",
                    },

                    {
                        name: "Show help",
                        href: "#",
                    },

                    {
                        name: "Contacs Us",
                        href: "#",
                    },
                ],

                sites: [
                    {
                        name: "DC",
                        href: "#",
                    },

                    {
                        name: "Mad magazine",
                        href: "#",
                    },

                    {
                        name: "DC Kids",
                        href: "#",
                    },

                    {
                        name: "DC Universe",
                        href: "#",
                    },

                    {
                        name: "DC Power Visa",
                        href: "#",
                    },
                ],
            }
        }
    }
</script>

<style lang="scss" scoped>
    footer {
        background-image: url("/public/img/footer-bg.jpg");
        background-size: cover;
        padding: 2rem;
        overflow: hidden;

        li a {
            color: grey;
            font-size: 0.7rem;
            font-family: Arial, Helvetica, sans-serif;
            text-decoration: none;
            transition: 0.2s ease-in-out;

            &:hover {
                color: white;
                transition: 0.2s ease-in-out;
            }
        }

        .logo-footer {
            top: -100px;
        }
    } 
</style>