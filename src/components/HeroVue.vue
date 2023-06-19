<template>
    <section class="hero">
        <div class="hero__grid">
            <div class="hero__item hero__item_1">
                <div class="hero__text-outer hero__text-outer_lg">
                    <span class="hero__text">
                        Мы официальные
                    </span>
                    <span class="hero__text_center">
                        дистрибьютеры
                    </span>
                    <span class="hero__text">
                        Весь товар в наличии
                    </span>
                </div>
            </div>
            <div class="hero__item hero__item hero__item_2">
                <div class="hero__text-outer">
                    <div class="hero__text-wrapper">
                        <span class="hero__text">Шкатулки</span>
                        <span class="hero__text">Для часов с автоподзаводом</span>
                    </div>
                    <button class="hero__button">Выбрать</button>
                </div>
            </div>
            <div class="hero__item hero__item hero__item_3">
                <div class="hero__text-outer">
                    <div class="hero__text-wrapper">
                        <span class="hero__text">Шкатулки</span>
                        <span class="hero__text">Для хранения часов</span>
                    </div>
                    <button class="hero__button">Выбрать</button>
                </div>
            </div>
            <div class="hero__item hero__item hero__item_4">
                <div class="hero__text-outer">
                    <div class="hero__text-wrapper">
                        <span class="hero__text">Шкатулки</span>
                        <span class="hero__text">Для украшений</span>
                    </div>
                    <button class="hero__button">Выбрать</button>
                </div>
            </div>
            <div class="hero__item hero__item hero__item_5">
                <div class="hero__text-outer">
                    <div class="hero__text-wrapper">
                        <span class="hero__text">Сейфы</span>
                        <span class="hero__text">Для часов</span>
                    </div>
                    <button class="hero__button">Выбрать</button>
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="sass" scoped>
.hero
    &__grid
        display: grid
        grid-template-columns: 1fr 1fr
        grid-template-rows: 516px 460px 460px
    &__item
            background-repeat: no-repeat
            background-size: cover
            &_1
                grid-column: 1/3
                background-image: url('/images/hero.png')
                background-repeat: no-repeat
                background-size: cover
            &_2
                background-image: url('/images/hero-2.png')
            &_3
                background-image: url('/images/hero-3.png')
            &_4
                background-image: url('/images/hero-4.png')
            &_5
                background-image: url('/images/hero-5.png')
    &__text-outer
        height: 100%
        width: fit-content
        margin-right: auto
        color: #fff
        font-weight: bold
        text-transform: uppercase
        font-size: 20px
        display: flex
        flex-direction: column
        justify-content: flex-end
        padding: 0 0 100px 55px
        &_lg
            width: 40%
            font-size: 36px
            margin-left: auto  
            margin-right: 0 
            justify-content: center   
            padding: 0 30px 0 0    
            gap: 25px
  
    &__text
        line-height: 1.3
        &_center
            align-self: center
    &__text-wrapper
        margin-block-end: 10px
    &__button
        width: fit-content
        color: inherit
        padding: 15px 35px
        background-color: #0c2362
        font-weight: bold
        text-transform: uppercase
</style>