<script setup>
import { ref } from 'vue';

const items = ref([
    'altitude',
    'aubolex',
    'avante',
    'bartz',
    'jebely',
    'wolf'
])
</script>

<template>
    <section class="fabricators">
        <h2 class="fabricators__title">Производители</h2>
        <ul class="fabricators__list">
            <li v-for="item,i in items" :key="i" class="fabricators__item">
                <img :src="'/images/'+item+'.png'" :alt="item">
            </li>
        </ul>
    </section>
</template>

<style lang="sass" scoped>
.fabricators
    &__title
        font-size: 38px
        text-transform: uppercase
        font-weight: normal
        color: #cdad78
        text-align: center
        margin-block: 20px
    &__list
        display: flex
        justify-content: space-between
        align-items: stretch
        gap: 24px
    &__item
        padding: 30px
        background-color: #efefef
        display: flex
        align-items: center
</style>