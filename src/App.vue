<template>
  <div>
    <h1>Studio Ghibli Films</h1>
    <div class="main-container">
      <film-list :films='films'></film-list>

    </div>
  </div>
</template>

<script>
import FilmList from "./components/FilmList.vue"


export default {
  name: 'app',
  data() {
    return {
      films: [],
      selectedFilm: null
    };
  },
  mounted() {
    fetch('https://ghibliapi.herokuapp.com/films')
    .then(response => response.json())
    .then(films => this.films = films)
  },

  components: {
    "film-list": FilmList
  }





}
</script>

<style>

</style>
