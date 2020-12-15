<template>
  <div id="app">

<div class="container-fluid">
    <div class="row justify-content-center mb-5">
      <div class="col mt-5" v-for="(item, index) of member" :key="index"> 
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
        nombre: "Karen Julieth Camargo Flórez",
        descripcion: "Ingeniera electrónica y Tecnologa en electrónica Industrial de las Unidades Tecnológicas de Santander," 
        + " entre sus pasatiempos favoritos se encuentra la fotografía y prácticar volleyball 🏐. Reside actualmente en la ciudad de Bucaramanga",
        rol: "Arquitecto de Software",
        imagen:"https://imgur.com/0r53PYm.jpg",
      },
      {
        codigo: 2,
        nombre: "Manuel José Hernández Rivas",
        descripcion: "Estudiante de ingeniería en sistemas computacionales y telemática. Programador java y desarrollador de"
        + " aplicaciones android nativas. Entré los pasatiempos están la lectura, la fotografía y el arte digital.",
        rol:"Desarrollador Backend",
        imagen:"https://imgur.com/c4VZpFz.jpg",
      },
      {
        codigo: 3,
        nombre: "Team J",
        descripcion: "Ingeniero Mecatronico, Nacido en Barrancabermeja, Santander,"
        + "Colombia curioso de nacimiento y apasionado por los videojuegos",
        rol:"Tester",
        imagen:"https://imgur.com/6dUC1Ub.jpg",
      },
      {
        codigo: 4,
        nombre: "Alex David Ospina Gonzalez",
        descripcion: "Estudiante de Español y Filología Clásica de la Universidad Nacional de Colombia," 
        + " tecnólogo en Gestión Bancaria y de Entidades Financieras del Servicio Nacional de Aprendizaje - SENA, gestor de prevención de fraudes del Banco Falabella Colombia.",
        rol:"Desarrollador Backend",
        imagen:"https://imgur.com/xJZp92x.jpg",
      },
      {
        codigo: 5,
        nombre: "Julio Cesar Cuervo Diaz",
        descripcion: "Ingeniero Mecatronico - Universidad Santo Tomas Bucaramanga, Nacido en Barrancabermeja, Santander,"
        + "Colombia curioso de nacimiento y apasionado por los videojuegos",
        rol:"Desarrollador Frontend",
        imagen:"https://imgur.com/QCkZqVk.jpg",
      },
    ]
  }
}
}

</script>

