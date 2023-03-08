<template>
    <div class="personal-data">
        <div class="personal-data__left">
            <span class="personal-data__left__text">Hola</span>
            <h3 class="personal-data__left__name">Soy Goku</h3>
            <p class="personal-data__left__description">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Officiis
                eligendi quibusdam voluptate non maxime
                natus consectetur.</p>

            <!--Import base component VButtonMain -->
            <v-button-main texto="Contactar" />
        </div>

        <div class="personal-data__right">
            <img src="@/assets/goku.png">
        </div>
    </div>
</template>

<script>

import VButtonMain from '@/components/base/VButtonMain'

export default {
    name: 'ThePersonalData',
    components: {
        VButtonMain
    }
}
</script>

<style lang="scss" scoped></style>