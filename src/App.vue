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
  <header class="header-section">
    <AppHeader />
  </header>
  <main class="main-section">
    <AppMain />
  </main>
  <footer class="footer-section">
    <AppFooter />
  </footer>

</template>

<style scoped>
.header-section {
  background-color: white;
  width: 100%;
  margin: 0;
  height: 5rem;
}

.main-section {
  width: 100%;
  margin: 0;
}

.footer-section {
  background-color: rgb(75, 75, 75);
  width: 100%;
  margin: 0;
  height: 5rem;
}
</style>
