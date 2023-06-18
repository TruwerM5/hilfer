
<script setup>
const routes = [
    { title: 'Для часов', path: '/'},
    { title: 'Для украшений', path: '/'},
    { title: 'Для сигар', path: '/'},
    { title: 'Для мужчин', path: '/'},
    { title: 'Для запонок', path: '/'},
    { title: 'Часы экслюзив', path: '/'},
    { title: 'Со скидкой', path: '/'},
    { title: 'Акции', path: '/'},
    { title: 'Отзывы', path: '/'},
]
</script>
<template>
    <header class="header">
        <div class="header__inner">
            <div class="header__top">
                <ul class="header__top-list">
                    <li class="header__top-item">Фирменная гарантия</li>
                    <li class="header__top-item">Бесплатная доставка</li>
                    <li class="header__top-item">Подлинные товары</li>
                    <li class="header__top-item">Самые низкие цены</li>
                </ul>
            </div>
            <div class="header__main">
                <router-link to="/" class="header__logo">
                    <img src="/images/logo.png" alt="Hilfer Logo">
                </router-link>
                <button class="header__button">
                    <img src="/images/search-icon.png" alt="Search">
                </button>
                <button class="header__button">
                    <img src="/images/user-icon.png" alt="User">
                </button>
                <button class="header__button">
                    <img src="/images/cart-icon.png" alt="Cart">
                </button>
            </div>
            <ul class="header__bottom">
                <router-link v-for="item,i in routes" :key="i" :to="{path: item.path}">
                    {{ item.title }}
                </router-link>
            </ul>
        </div>
    </header>
</template>


<style lang="sass" scoped>
.header
    &__top
        padding-inline: 300px
        background-color: #e0e0e0
    &__top-list
        height: 60px
        display: flex
        align-items: center
        gap: 75px
    &__main
        height: 114px
        display: flex
        gap: 70px
        align-items: center
        padding-inline: 300px
    &__logo
        margin-right: auto
    &__button
        background-color: transparent
    &__bottom
        height: 60px
        display: flex
        align-items: center
        padding-inline: 300px
        background-color: #2d4257
        color: #fff
        text-transform: uppercase
        font-weight: bold
        gap: 40px
</style>