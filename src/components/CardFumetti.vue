<script>
export default {
    name: 'CardFumetti',
    props: ["singoloFumetto"],

    data() {
        return {

        }
    }
}

</script>

<template>

    <div class="single-card">
        <img :src="singoloFumetto.thumb" alt="">
        <h6 class="mt-3">{{ singoloFumetto.series }}</h6>
    </div>

</template>

<!-- in questo caso e` corretto scoped ??? -->
<style scoped>
.single-card {
    width: calc(100% / 6 - 2rem);
    margin: 1rem 1rem;
    padding: 0.5rem;
    text-align: center;
}

img {
    width: 10rem;
    height: 10rem;
}
</style>