<template>
    <div class="main-card" :style="{ background: color }">
        <h4 class="main-card__title">{{ title }}</h4>
        <p class="main-card__text">{{ content }}</p>
    </div>
</template>

<script>
export default {
    name: 'VCardMain',
    props: {
        title: String,
        content: String,
        color: String,
    }
}
</script>

<style lang="scss" scoped>
@import '@/components/app.scss';

.main-card {
    width: 300px;
    padding: 2em;
    color: $color-white;
    margin: 10px;
    height: 150px;

    &__title {
        font-family: $ff-primary;
        font-size: 20px;
        margin-bottom: 1em;
    }

    &__text {
        font-family: $ff-secondary;
    }
}
</style>