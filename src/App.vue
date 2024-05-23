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
  <div class="header-section">
    <AppHeader />
  </div>
  <div class="main-section">
    <AppMain />
  </div>
  <div class="footer-section">
    <AppFooter />
  </div>

</template>

<style scoped>
.header-section {
  background-color: white;
  width: 100%;
  margin: 0;
  height: 5rem;
}

.main-section {
  background-color: red;
  width: 100%;
  margin: 0;
  height: calc(100vh - 10rem);
}

.footer-section {
  background-color: rgb(75, 75, 75);
  width: 100%;
  margin: 0;
  height: 5rem;
}
</style>
