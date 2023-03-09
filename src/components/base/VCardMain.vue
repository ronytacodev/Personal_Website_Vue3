<template>
    <div class="main-card" :style="{ background: color }">
        <h4>{{ titulo }}</h4>
        <p>{{ contenido }}</p>
    </div>
</template>

<script>
export default {
    name: 'VCardMain',
    props: {
        titulo: String,
        contenido: String,
        color: String,
    }
}
</script>

<style lang="scss" scoped></style>