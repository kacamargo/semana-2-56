<template>
  <div id="app">
    <services-section> </services-section>
    <div class="jumbotron jumbotron-fluid py-3" style="background: #f1f2f3">
      <h6 class="display-2 text-center">Noticias</h6>
      <p class="text-muted text-center lead m-0">En esta sección podrás encontrar las noticias más relevantes del sector seguros...</p>
      <div class="container-fluid">
        <news-section></news-section>
      </div>
    </div>
  </div>
  
</template>

<script>
import NewsSection from './components/NewsSection.vue'
import ServicesSection from './components/ServicesSection.vue'

export default {
  name: 'App',
  components: {
  ServicesSection,
  NewsSection,
  }
}
</script>

<style scoped>
  h6 {
    font-family: 'Roboto', sans-serif;
    color: #2a2e31;

  }
</style>