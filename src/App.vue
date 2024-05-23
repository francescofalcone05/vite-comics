<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter
  }
}
</script>

<template>
  <h1>appvue funziona</h1>
  <AppHeader />
  <AppMain />
  <AppFooter />

</template>

<style scoped></style>
