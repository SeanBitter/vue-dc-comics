<template>
    <div class="container">
        <div class="d-flex justify-content-between">
            <div class="d-flex align-items-center">
                <a href="#">
                    <img src="/img/dc-logo.png" alt="DC Comics" width="60" height="60">
                </a>
            </div>
            <div class="pt-5">
                <ul class="list-unstyled d-flex mb-0">
                    <li v-for="(link, i) in navBar" :key="i">
                        <a :href="link.href">{{ link.name }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'TheHeader',

        data() {
            return {
                navBar: [
                    {
                        name: "CHARACTERS",
                        href: "#",
                    },

                    {
                        name: "COMICS",
                        href: "#",
                    },

                    {
                        name: "MOVIES",
                        href: "#",
                    },

                    {
                        name: "TV",
                        href: "#",
                    },

                    {
                        name: "GAMES",
                        href: "#",
                    },

                    {
                        name: "COLLECTIBLES",
                        href: "#",
                    },

                    {
                        name: "VIDEOS",
                        href: "#",
                    },

                    {
                        name: "FANS",
                        href: "#",
                    },

                    {
                        name: "NEWS",
                        href: "#",
                    },

                    {
                        name: "SHOP",
                        href: "#",
                    },
                ],
            }
        }
    }
</script>

<style lang="scss" scoped>
@import "../assets/scss/variables";

    li a {
        text-decoration: none;
        color: black;

        &:hover {
            color: $primary;
        }
    }

    li {
        margin: 0 1rem;
        padding-bottom: 2rem;
        border-bottom: 4px solid transparent;

        &:hover {
            border-bottom: 4px solid $primary;
        }
    }
</style>