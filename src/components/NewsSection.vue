<template>
  <div>
    <div class="row mt-md-5 mt-sm-5 mt-xs-5">
      <div class="d-flex col-lg-6 col-xs-12" v-for="noticia in news" :key="noticia.id">
        <div class="shadow p-4 mb-4 bg-white " alt="Contenedor noticias">
          <div class="d-flex justify-content-center align-items-center">
            <div class="p-2" style="width:50%" >
              <img
                :src="noticia.image"
                class="img-fluid rounded"
                alt="Poster noticia"
              />
            </div>
            <div class="p-2" style="width:50%"  >
              <h5 class="text-center">{{ noticia.title }}</h5>
              <div class=" mx-auto" style="width: 30%; height: 0.25em; background: #78344c; "></div>
              <p class="my-2">{{ noticia.description }}</p>
              <div class="d-flex container-fluid justify-content-end p-2">
                <a
                  :href="noticia.source.url"
                  class="btn btn-outline-info"
                  target="_blank"
                  >Ver Noticia</a
                >
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";

export default {
  name: "NewsSection",
  data() {
    return {
      news: null,
    };
  },
  mounted() {
    axios
      .get(
        "https://gnews.io/api/v4/search?q=seguros&lang=es&country=col&max=4&token=9126da21db32f085084d4032b4646b4e"
      )
      .then((response) => {
        this.news = response.data.articles;
        console.log(this.news);
      });
  },
};
</script>
    
<style scoped>
h5 {
  font-family: 'Lato';
  margin-bottom: 20px;
}

</style>