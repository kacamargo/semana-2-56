<template>
    <div></div>
</template>

<script>
// import axios from 'axios'

export default {
    name: 'NewsSection',
    data(){
        return {
            movies: null
        }
    },
    mounted(){
        axios
        .get('https://gnews.io/api/v4/search?q=health&lang=es&country=col&max=4&token=9126da21db32f085084d4032b4646b4e')
        .then(response => {
            (this.movies = response)
            console.log(this.movies)
        }
        )
    }    
}
</script>
    
<style scoped>

</style>