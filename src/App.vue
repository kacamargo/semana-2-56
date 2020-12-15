<template>
  <div id="app">
    <div class="jumbotron jumbotron-fluid py-3" style="background: #f1f2f3">
      <h6 class="display-2 text-center">Noticias</h6>
      <p class="text-muted text-center lead">En esta sección podrás encontrar las noticias más relevantes del sector salud</p>
      <div class="container-fluid">
        <news-section></news-section>
      </div>
    </div>
  </div>
</template>

<script>
import NewsSection from "./components/NewsSection.vue";

export default {
  name: "App",
  components: {
    NewsSection,
  },
};
</script>

<style scoped>
  h6 {
    font-family: 'Roboto', sans-serif;
    color: #2a2e31;

  }
</style>