<template>
    <div class="thumbnails">
        <div v-for="movie in movies" :key="movie.id">
            <div class="poster" @click="changeCurrent(movie)">
                <img :src="movie.poster" height="200">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: ['movies'],
    methods: {
        changeCurrent(movie) {
            this.$emit('choose-movie', movie)
        }
    }
}
</script>