<template>
    <a class="main-btn" href="#" :style="{ color: colorTexto, background: colorFondo }">
        {{ texto }}
    </a>
</template>

<script>
export default {
    name: 'VButtonMain',
    props: {
        texto: String,
        colorTexto: String,
        colorFondo: String
    }
}
</script>

<style lang="scss" scoped>
@import '@/components/app.scss';

.main-btn {
    padding: 7px 20px 7px 20px;
    font-family: $ff-secondary;
    border: 1px solid;
    margin: 5px;
    text-decoration: none;
}
</style>