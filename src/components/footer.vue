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

<footer class="page-footer bg-secondary text-white pt-4">

        <!-- Footer Text -->
        <div class="container-fluid text-center text-md-left">

            <!-- Grid row -->
            <div class="row">

                <!-- Grid column -->
                <div class="col-md-6 mt-md-0 mt-3">

                    <!-- Content -->
                    <h5 class="text-uppercase font-weight-bold">Acerda de</h5>
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Expedita sapiente sint, nulla, nihil
                        repudiandae
                        commodi voluptatibus corrupti animi sequi aliquid magnam debitis, maxime quam recusandae harum
                        esse fugiat.
                        Itaque, culpa?</p>

                </div>
                <!-- Grid column -->

                <hr class="clearfix w-100 d-md-none pb-3">

                <!-- Grid column -->
                <div class="members col-md-6 mb-md-0 mb-3">

                    <!-- Content -->
                    <h5 class="text-uppercase font-weight-bold">Equipo de trabajo</h5>
                    <p>Karen Julieth Camargo Flórez - Arquitecto de Software - Kjcamargo19@gmail.com</p>
                    <p>Manuel José Hernández Rivas - Desarrollador BackEnd - manuel_hzr@outlook.com</p>
                    <p>Alex David Ospina Gonzalez - Desarrollador BackEnd - ganjalex64@hotmail.com</p>
                    <p>Julio Cesar Cuervo Diaz  - Desarrollador FrontEnd - Ing.cuervodiaz@gmail.com</p>

                </div>
                <!-- Grid column -->

            </div>
            <!-- Grid row -->

        </div>
        <!-- Footer Text -->

        <!-- Copyright -->
        <div class="footer-copyright text-center py-1 bg-dark">© 2020 Copyright: DAD
        </div>
        <!-- Copyright -->

    </footer>

</template>

<script>
export default {
    name:"footer"
}
</script>

<style>

.members h5 {
    font-size: 1.5rem;
}

.members p {
    font-size: 1.2rem;
}

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