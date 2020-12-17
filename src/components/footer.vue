<template>

<footer class="page-footer bg-secondary text-white pt-4">

        <div class="container-fluid text-center text-md-left">
            <div class="row">
                <div class="col-md-6 mt-md-0 mt-3">

                    <h5 class="text-uppercase font-weight-bold">Acerda de</h5>
                    <p>Desarrollado por TEAM 56 UTP. Somos una compañía de desarrollo web encaminada a la innovación en la presentación y servicios de páginas WEB.</p>
                    <p>Dirección principal: Avenida Siempre Viva # 123, Bogotá, Colombia.</p>
                    <p>Teléfono: (1)987-6543</p>
                    <p>Celular: (+57)3987654321</p>
                    <a href="https://github.com/kacamargo/semana-2-56.git">GitHub</a>
                </div>

                <hr class="clearfix w-100 d-md-none pb-3">

                <div class="col-md-6 mb-md-0 mb-3">
                    <h5 class="text-uppercase font-weight-bold">Equipo de trabajo</h5>
                    <p>Karen Julieth Camargo Flórez - Arquitecto de Software - Kjcamargo19@gmail.com</p>
                    <p>Manuel José Hernández Rivas - Desarrollador BackEnd - manuel_hzr@outlook.com</p>
                    <p>Alex David Ospina Gonzalez - Desarrollador BackEnd - ganjalex64@hotmail.com</p>
                    <p>Julio Cesar Cuervo Diaz  - Desarrollador FrontEnd - Ing.cuervodiaz@gmail.com</p>
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

h5, a {
    font-size: 1.5rem;
}

p {
    font-size: 1.15rem;
}

a {
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