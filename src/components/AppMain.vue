<script>
import AppMainFirst from './AppMainFirst.vue';
import AppMainSecond from './AppMainSecond.vue';
import AppMainThird from './AppMainThird.vue';


export default {
    components: {
        AppMainFirst,
        AppMainSecond,
        AppMainThird
    }
}
</script>

<template>
    <div class="first-section">
        <AppMainFirst />
    </div>
    <div class="second-section">
        <AppMainSecond />
    </div>
    <div class="third-section">
        <AppMainThird />
    </div>
</template>

<style scoped>
.first-section {
    min-height: 5rem;
    background-color: black;
}

.second-section {
    height: 5rem;
    background-color: blue;
}

.third-section {
    height:20rem;
    background-image: url(../assets/img/footer-bg.jpg);
}
</style>