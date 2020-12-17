<template>
  <div id="app">
    <cabecera> </cabecera>
    
    <!-- Seccion servicios -->
    <h6 class="display-2 text-center mt-2" id="services" >Nuestros Servicios</h6>
    <services-section> </services-section>

    <!-- Seccion noticias -->
    <div class="jumbotron jumbotron-fluid py-3" style="background: #f1f2f3" id="noticias">
      <h6 class="display-2 text-center">Noticias</h6>
      <p class="text-muted text-center lead m-0">En esta sección podrás encontrar las noticias más relevantes del sector seguros...</p>
      <div class="container-fluid" >
        <news-section></news-section>
      </div>
    </div>

    <!-- Seccion Team -->
    <div class="container-fluid" id="equipo">
      <h6 class="display-2 text-center" style="font-family: 'Roboto', sans-serif;">Conoce Nuestro Equipo</h6>
      <p class="text-muted text-center lead mb-0">¡Creemos sinceramente que la tecnología tiene un potencial casi ilimitado para cambiar nuestro mundo!</p>
        <div class="row justify-content-center mb-5">
          <div class="col-md mt-4 d-flex justify-content-around" v-for="(item, index) of member" :key="index"> 
            <team-card v-bind:member="item"></team-card>
          </div>
        </div>
    </div>

    <pie></pie>
  </div> 
</template>

<script>
import cabecera from './components/header.vue'
import NewsSection from './components/NewsSection.vue'
import ServicesSection from './components/ServicesSection.vue'
import TeamCard from './components/TeamCard.vue' 
import pie from './components/footer'


export default {
  name: 'App',
  components: {
  cabecera,
  ServicesSection,
  NewsSection,
  TeamCard,
  pie
  },
data(){
  return{
    member:[
      {
        codigo: 1,
        nombre: "Karen Julieth Camargo Florez",
        descripcion: "Ingeniera Electrónica y Tecnóloga en Electrónica Industrial de las Unidades Tecnológicas de Santander," 
        + " entre sus pasatiempos favoritos se encuentra la fotografía y prácticar voleibol.",
        rol: "Arquitecto de Software",
        imagen:"https://imgur.com/0r53PYm.jpg",
      },
      {
        codigo: 2,
        nombre: "Manuel José Hernández Rivas",
        descripcion: "Estudiante de Ingeniería en Sistemas Computacionales y Telemática. Programador Java y desarrollador de"
        + " aplicaciones Android nativas. Entré los pasatiempos están la lectura, la fotografía y el arte digital.",
        rol:"Desarrollador Backend",
        imagen:"https://imgur.com/c4VZpFz.jpg",
      },
      {
        codigo: 3,
        nombre: "team 56 utp",
        descripcion: ">>'Ninguno de nosotros es tan inteligente como todos nosotros' - Ken Blanchard >>'De la conducta de cada uno depende el destino de todos' - Alejandro Magno.",
        rol:"trabajo en equipo",
        imagen:"https://imgur.com/6dUC1Ub.jpg",
      },
      {
        codigo: 4,
        nombre: "Alex David Ospina Gonzalez",
        descripcion: "Estudiante de Español y Filología Clásica de la Universidad Nacional de Colombia," 
        + " Tecnólogo en Gestión Bancaria y de Entidades Financieras del Servicio Nacional de Aprendizaje - SENA, Gestor de prevención de fraudes del Banco Falabella Colombia.",
        rol:"Desarrollador Backend",
        imagen:"https://imgur.com/xJZp92x.jpg",
      },
      {
        codigo: 5,
        nombre: "Julio Cesar Cuervo Diaz",
        descripcion: "Ingeniero Mecatrónico - Universidad Santo Tomás Bucaramanga, Nacido en Barrancabermeja, Santander,"
        + "Colombia. Curioso de nacimiento y apasionado por los videojuegos.",
        rol:"Desarrollador Frontend",
        imagen:"https://imgur.com/QCkZqVk.jpg",
      }
    ]
  }
}
}

</script>

<style scoped>
  h6 {
    font-family: 'Roboto', sans-serif;
    color: #2a2e31;
  }
</style>

