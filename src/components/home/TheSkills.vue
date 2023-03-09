<template>
    <div class="skills">
        <h3 class="skills__title">Mis habilidades</h3>

        <p class="skills__text">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Illum, totam. Dolore eligendi
            ipsam iste dolorem
            laudantium
            accusantium.</p>

        <div class="skills__items">
            <div v-for="skill in skills" :key="skill.id" class="skills__item">
                <v-card-main :title="skill.title" :content="skill.content" :color="skill.color" />
            </div>
        </div>

    </div>
</template>

<script>

import VCardMain from '@/components/base/VCardMain'

export default {
    name: 'TheSkills',
    data() {
        return {
            skills: [
                { 'id': 0, 'title': 'Fuerza', 'content': 'Lorem ipsum dolor sit, amet consectetur adipisicing elit', color: '#ff9f1a' },

                { 'id': 1, 'title': 'Velocidad', 'content': 'Lorem ipsum dolor sit, amet consectetur adipisicing elit', color: '#18dcff' },

                { 'id': 2, 'title': 'Teletransportación', 'content': 'Lorem ipsum dolor sit, amet consectetur adipisicing elit', color: '#c56cf0' },

                { 'id': 3, 'title': 'UltraInstinto', 'content': 'Lorem ipsum dolor sit, amet consectetur adipisicing elit', color: '#3ae374' }
            ]
        }
    },
    components: {
        VCardMain
    }

}
</script>

<style lang="scss" scoped>
@import '@/components/app.scss';

.skills {
    background: $color1;
    padding: 4em;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;

    &__title {
        font-family: $ff-primary;
        color: $color-white;
        margin-bottom: 1em;
        font-size: 24px;
    }

    &__text {
        font-family: $ff-secondary;
        color: $color-white;
        margin-bottom: 1em;
    }

    &__items {
        display: grid;
        grid-template-columns: 400px 400px;
    }
}
</style>