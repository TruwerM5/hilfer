<script setup>
defineProps({
    img: {
        type: String,
    },
    name: {
        type: String,
    },
    collection: {
        type: String,
    },
    price: {
        type: Number,
    }
})
</script>

<template>
    <li class="product">
        <div class="product__inner">
            <div class="product__img-wrapper">
                <img :src="img" :alt="name">
            </div>
            <div class="product__details">
                <p class="product__name">{{ name }}</p>
                <span class="product__collection">{{ collection }}</span>
                <span class="product__price">{{ price }} руб.</span>
            </div>
        </div>
    </li>
</template>

<style lang="sass" scoped>
.product
    &__img-wrapper
        padding: 60px
        background-color: #e9e9e9
    &__details
        text-align: center
        padding-block: 30px
        display: flex
        flex-direction: column
        gap: 10px
    &__collection
        font-size: 12px
        color: #464646
</style>