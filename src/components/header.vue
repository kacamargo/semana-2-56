<template>
  <header class="site-header inicio">
        <div class="contenedor contenido-header">
            <div class="barra">
                <a href="#">
                    <img src="../assets/logoHeader.svg" alt="Logotipo alpha">
                </a>
                <nav class="navegacion">
                    <a href="#">Inicio</a>
                    <a href="#">Servicios</a>
                    <a href="#">Noticias</a>
                    <a href="#">Equipo</a>
                </nav>
            </div>

            <h1>Lorem ipsum dolor sit, consectetur adipisicing elit. </h1>
        </div> <!-- contenedor-->
    </header>
</template>

<script>
export default {
  name: "cabecera"
};
</script>

<style>

html{
    box-sizing: border-box;
    font-size: 62.5%; /** Reset para REMS -62.5% -10px de 16px **/
}

.contenedor{
    max-width: 120rem;
    margin: 0 auto;
}

.site-header{
    background-color: #333333;
    padding: 1rem 0 3rem 0;
}

.site-header.inicio{
    background-image: url(../assets/header1.jpg);
    background-position: center center;
    background-size: cover;
    height: 100vh;
    min-height: 60rem;
}

.contenido-header{
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
}

.contenido-header h1{
    color: white;
    padding-bottom: 2rem;
    max-width: 60rem;
    line-height: 2;
}

.barra{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 3rem;
}

/* Navegacion */
.navegacion a {
    color: white;
    text-decoration: none;
    font-size: 1.8rem;
    margin-right: 2rem;
}

.navegacion a:hover{
    color: #71B100;
}

.navegacion a:last-of-type{
    margin: 0;
}
</style>