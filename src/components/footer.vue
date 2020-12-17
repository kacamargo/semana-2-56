<template>

<footer class="page-footer bg-secondary text-white pt-4">

        <div class="container-fluid text-center text-md-left">
            <div class="row">
                <div class="col-md-6 mt-md-0 mt-3">

                    <h5 class="text-uppercase font-weight-bold">Acerca de</h5>
                    <p>Desarrollado por TEAM 56 UTP. Somos una compañía de desarrollo web encaminada a la innovación en la presentación y servicios de páginas WEB.</p>
                    <p class="mb-0">Dirección principal: Avenida Siempre Viva # 123, Bogotá, Colombia.</p>
                    <p class="mb-0">Teléfono: (1)987-6543</p>
                    <p class="mb-0">Celular: (+57)3987654321</p>
                    <a href="https://github.com/kacamargo/semana-2-56.git" target="_blanck">GitHub</a>
                </div>

                <hr class="clearfix w-100 d-md-none pb-3">

                <div class="col-md-6 mb-md-0 mb-3">
                    <h5 class="text-uppercase font-weight-bold text-center mb-4">Contáctanos</h5>
                    <p class="mb-0">Karen Camargo - Arquitecto de Software - kjcamargo19@gmail.com</p>
                    <p class="mb-0">Manuel Hernández - Desarrollador BackEnd - manuel_hzr@outlook.com</p>
                    <p class="mb-0">Alex Ospina - Desarrollador BackEnd - ganjalex64@hotmail.com</p>
                    <p class="mb-0">Julio Cuervo - Desarrollador FrontEnd - ing.cuervodiaz@gmail.com</p>
                </div>
            </div>
        </div>

        <div class="footer-copyright text-center py-1 bg-dark">&copy; 2020 Copyright: Seguros Alpha &#174; - Todos los derechos reservados.</div>

    </footer>

</template>

<script>
export default {
    name:"footer"
}
</script>

<style>

.page-footer h5, a {
    font-size: 1rem;
}

.page-footer p {
    font-size: 0.9rem;
}

.page-footer a {
  color: white;
  text-decoration: none;
  margin-right: 2rem;
}

a:hover{
    color: #333333;
}

a:last-of-type {
  margin: 0;
}

</style>