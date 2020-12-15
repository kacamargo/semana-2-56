<template>
    <div class="card shadow">
        <div class="d-flex justify-content-center p-2" style=" margin-top:1.5em">
            <img v-bind:src="member.imagen" alt="Team photo shoot" class="rounded img-fluid">
        </div>

        <div class="card-body">
            <p class="card-title text-center h4 text-uppercase mb-3" style="color: #78344c; font-family:'Bebas Neue', cursive;">{{ member.nombre }}</p>
            <div class=" mx-auto" style="width: 30%; height: 2px; background: #78344c; "></div>
            <p class="card-text text-center h6 py-2" style=""><small>{{ member.descripcion }}</small></p>
        </div>
        <div class="card-footer text-uppercase my-0" style="background:#78344c; height:3em">
            <p class= "text-center m-0 small" style="color: #ffffff;" >{{ member.rol}}</p>
        </div>
    </div>
</template>

<script>
    export default {
        name: "TeamCard",
        props: {
            member: Object
        }
    }
</script>

<style scoped>
</style>
