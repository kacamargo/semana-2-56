<template>
  <div id="app">

<div class="container-fluid">
  <h6 class="display-2 text-center" style="font-family: 'Roboto', sans-serif;">Conoce Nuestro Equipo</h6>
  <p class="text-muted text-center lead mb-0">¡Creemos sinceramente que la tecnología tiene un potencial casi ilimitado para cambiar nuestro mundo!</p>
    <div class="row justify-content-center mb-5">
      <div class="col-md mt-4 d-flex justify-content-around" v-for="(item, index) of member" :key="index"> 
        <team-card v-bind:member="item"></team-card>

      </div>
    </div>
</div>

  </div>
</template>

<script>

import TeamCard from './components/TeamCard.vue' 

export default {
  name: 'App',
  components:{
    TeamCard
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
        nombre: "",
        descripcion: ">>'Ninguno de nosotros es tan inteligente como todos nosotros' - Ken Blanchard >>'De la conducta de cada uno depende el destino de todos' - Alejandro Magno.",
        rol:"",
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
      },
    ]
  }
}
}

</script>