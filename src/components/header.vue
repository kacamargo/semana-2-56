<template>
  <header class="site-header inicio">
    <!-- contenedor-->
    <div>
      <transition-group  name="fade" tag="div">
        <div class="caja" v-for="i in [currentIndex]" :key="i">
          <img class="imageside" :src="currentImg" />
          <div class="texto" v-text="currentText"></div>
        </div>
      </transition-group>

      <div class="contenedor contenido-header">
          <div class="barra">
            <a href="#"> <img src="../assets/logoHeader.svg" alt="Logotipo alpha"> </a>
            <nav class="navegacion">
              <a href="#">Inicio</a>
              <a href="#">Servicios</a>
              <a href="#">Noticias</a>
              <a href="#">Equipo</a>
            </nav>
          </div>
        </div>

      <a class="prev" @click="prev" href="#">&#10094;</a>
      <a class="next" @click="next" href="#">&#10095;</a>
    </div>
  </header>

</template>

<script>
export default {
  name: "cabecera",

data() {
    return {
      images: [
        "https://i.imgur.com/27nlDg0.jpg",
        "https://i.imgur.com/vtHPO89.jpg",
        "https://i.imgur.com/lJBbiBI.jpg",
      ],
      titles: ["Image 1", "Image 2", "Image 3",],
      timer: null,
      currentIndex: 0,
    };
  },

  mounted: function () {
    this.startSlide();
  },

  methods: {
    startSlide: function () {
      this.timer = setInterval(this.next, 6000);
    },

    next: function () {
      this.currentIndex += 1;
    },
    prev: function () {
      this.currentIndex -= 1;
    },
  },

  computed: {
    currentImg: function () {
      return this.images[Math.abs(this.currentIndex) % this.images.length];
    },
    currentText: function () {
      return this.titles[Math.abs(this.currentIndex) % this.images.length];
    },
  },

};
</script>

<style>

html{
    box-sizing: border-box;
    font-size: 62.5%; /** Reset para REMS -62.5% -10px de 16px **/
}

.caja {
  position: relative;
  height: max-content;
}

.texto {
  position: absolute;
  top: 80%;
  left: 10%;
  font-size: 30px;
  color: white;
  text-shadow: 2px 2px 2px #333333;
}

.imageside{
    max-height: 100vh;
}

.fade-enter-active,
.fade-leave-active {
  transition: all 0.9s ease;
  overflow: hidden;
  visibility: visible;
  position: absolute;
  width: 100%;
  opacity: 1;
}

.fade-enter,
.fade-leave-to {
  visibility: hidden;
  width: 100%;
  opacity: 0;
}

img {
  height: 100%;
  width: 100%;
  position: center center;
}

.prev,
.next {
  cursor: pointer;
  position: absolute;
  top: 40%;
  width: auto;
  padding: 16px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.7s ease;
  border-radius: 0 4px 4px 0;
  text-decoration: none;
  user-select: none;
}

/* Position the "next button" to the right */
.next {
  right: 0;
}

.prev {
  left: 0;
}

/* On hover, add a black background color with a little bit see-through */
.prev:hover,
.next:hover {
  background-color: rgba(0, 0, 0, 0.9);
}



.contenedor {
  min-width: 80%;
  margin: 0 auto;
  position: absolute;
  top: 10px;
  left: 10%;
}

.site-header {
  background-color: #333333;
  padding: 0 0 3rem 0;
  position: relative;
}


.site-header.inicio{
    /*background-image: url(../assets/header1.jpg);*/
    background-position: center center;
    background-size: cover;
    height: 100vh;
}

.contenido-header {
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.contenido-header h1 {
  color: white;
  padding-bottom: 2rem;
  max-width: 60rem;
  line-height: 2;
}


.barra {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-top: 3rem;
  align-items: flex-end;
  text-shadow: 3px 3px 3px #333333;
}



/* Navegacion */
.navegacion a {
  color: white;
  text-decoration: none;
  font-size: 1.8rem;
  margin-right: 2rem;
}

.navegacion a:hover {
  color: #333333;
}

.navegacion a:last-of-type {
  margin: 0;
}
</style>