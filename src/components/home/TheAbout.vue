<template>
    <div class="about">
        <div class="about__content">
            <div class="about__content__left">

                <img class="about__content__left__img" src="@/assets/goku2.jpg">

            </div>

            <div class="about__content__right">
                <h3 class="about__content__right__title">Sobre Mi</h3>

                <p class="about__content__right__text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Mollitia
                    saepe, reprehenderit amet reiciendis velit neque. Deserunt rem dolorum, veniam dolores eius tenetur
                    animi odio voluptatibus expedita minima inventore et accusantium.</p>

                <div class="about__content__right__controls">

                    <!--Import base component VButtonMain -->
                    <v-button-main texto="Linkedin" color-texto="#ff9f1a" color-fondo="#212121" />
                    <v-button-main texto="Github" color-texto="#212121" color-fondo="#ff9f1a" />

                </div>
            </div>
        </div>
    </div>
</template>

<script>

import VButtonMain from '@/components/base/VButtonMain'

export default {
    name: 'TheAbout',
    components: {
        VButtonMain
    }
}
</script>

<style lang="scss" scoped>
@import '@/components/app.scss';

.about {
    display: flex;
    justify-content: center;
    align-items: center;
    border: 1px solid;
    padding: 4em 0 4em 0;
    background: $color1;
    opacity: .90;

    &__content {
        width: 50%;
        display: flex;
        justify-content: center;
        align-items: center;

        &__left {
            border: 1px solid $color2;
            width: 150px;
            height: 100px;
            margin-right: 3em;

            &__img {
                width: 100%;
                height: 100%;
                position: relative;
                left: 20px;
                top: -20px;
            }
        }

        &__right {
            display: block;
            width: 50%;
            color: $color-white;

            &__title {
                font-family: $ff-primary;
                font-size: 20px;
                border-bottom: 1px solid $color2;
                margin-bottom: 1em;
                padding-bottom: 1em;
            }

            &__text {
                font-size: 15px;
                font-family: $ff-secondary;
                margin-bottom: 1.5em;
            }
        }
    }
}
</style>