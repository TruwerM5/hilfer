<script setup>
import HeroVue from '../components/HeroVue.vue';
import CarouselVue from '../components/CarouselVue.vue';
import FabricatorsVue from '../components/FabricatorsVue.vue';
import { ref } from 'vue';

const bestsellers = ref([
    {
        img: 'casket-1.png',
        name: 'Шкатулка для подзавода (клён)',
        collection: 'Коллекция TRADITION',
        price: 115000
    },{
        img: 'casket-2.png',
        name: 'Шкатулка для подзавода (клён)',
        collection: 'Коллекция TRADITION',
        price: 98000
    },{
        img: 'casket-3.png',
        name: 'Шкатулка для подзавода 8 часов (клён)',
        collection: 'Коллекция TRADITION',
        price: 98000
    },
]);

const discounts = ref([
{
        img: 'casket-1.png',
        name: 'Шкатулка для подзавода (клён)',
        collection: 'Коллекция TRADITION',
        price: 115000
    },{
        img: 'casket-2.png',
        name: 'Шкатулка для подзавода (клён)',
        collection: 'Коллекция TRADITION',
        price: 98000
    },{
        img: 'casket-3.png',
        name: 'Шкатулка для подзавода 8 часов (клён)',
        collection: 'Коллекция TRADITION',
        price: 98000
    },
])
</script>

<template>
    <HeroVue />
    <CarouselVue :title="'Бестселлеры'" :items="bestsellers" />
    <CarouselVue :title="'Товары со скидкой'" :items="bestsellers" />
    <FabricatorsVue />
</template>