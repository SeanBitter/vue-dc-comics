<template>
    <div class="py-4 card-section">
        <div>
            <img :src="imgUrl" :alt="cardTitle" class="img-cards">
        </div>
        <div class="pt-3">{{ cardTitle }}</div>
    </div>
</template>

<script>
    export default {
        name: 'DcCard',

        props: {
            cardTitle: String,
            imgUrl: String,
            cardPrice: String,
            cardType: String,
        }
    }
</script>

<style lang="scss" scoped>

    .img-cards {
        max-height: 180px;
        max-width: 100%;
        aspect-ratio: 1;
    }
    .card-section {
        font-family: Arial, Helvetica, sans-serif;
    }

</style>