<template>

    <div class="card border-dark bg-light" style="height: 38em">
        <div class="d-flex justify-content-center p-2" style=" margin-top:1.5em">
            <img v-bind:src="member.imagen" alt="Team photo shoot" class="rounded">
        </div>

        <div class="card-body">
            <p class="card-title text-center h6 text-uppercase">{{ member.nombre }}</p>
            <p class="card-title text-center h6 text-uppercase"><small class="text-muted">{{ member.rol }}</small></p>
            <br>
            <p class="card-text text-center h6 "><small>{{ member.descripcion }}</small></p>
        </div>
        <div class="card-footer text-center">
            <small class="text-muted">12 - Dic - 2020</small>
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
