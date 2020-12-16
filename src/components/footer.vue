<template>
  <!-- <footer class="site-footer seccion">
        <div class="contenedor contenedor-footer">
            <nav class="navegacion">
                <a href="nosotros.html">Nosotros</a>
                <a href="anuncios.html">Anuncios</a>
                <a href="blog.html">Blog</a>
                <a href="contacto.html">Contacto</a>
            </nav>

            <p class="copyright">Todos los derechos reservados 2020 &copy;</p>
        </div>
  </footer> -->

</template>

<script>
export default {
    name:"footer"
}
</script>

<style>
.site-footer {
    background-color: #333333;
    margin: 0;
    position: absolute;
}

.seccion{
    margin-top: 2rem;
    margin-bottom: 2rem;
}

.contenedor{
    max-width: 120rem;
    margin: 0 auto;
}

.contenedor-footer {
    padding: 3rem 0;
    display: flex;
    justify-content: space-between;
}
.navegacion a {
    color: white;
    text-decoration: none;
    font-size: 1.8rem;
    margin-right: 2rem;
}

</style>