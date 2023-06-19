<script setup>
import ProductVue from './ProductVue.vue';
defineProps({
    title: {
        type: String, 
        required: true,
    },
    items: {
        type: Object,
        required: true,
    }
})
</script>

<template>
    <section class="carousel">
        <h2 class="carousel__title">{{ title }}</h2>
        <div class="carousel__inner">   
            <ul class="carousel__list">
                <!-- Product item here -->
                <ProductVue v-for="item in items" 
                :img="'/images/'+item.img" 
                :name="item.name" 
                :collection="item.collection"
                :price="item.price" />
            </ul>
        </div>
    </section>
</template>

<style lang="sass" scoped>
.carousel
    &__title
        font-size: 38px
        text-transform: uppercase
        font-weight: normal
        color: #cdad78
        text-align: center
        margin-block: 20px
    &__list
        display: flex
        gap: 24px
        justify-content: space-between
</style>