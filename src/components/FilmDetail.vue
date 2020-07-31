<template>
  <div v-if="film">
      <h2>{{film.title}}</h2>
      <ul>
          <li>Title: {{film.title}}</li>
          <li>Director: {{film.director}}</li>
      </ul>

  </div>
</template>

<script>
export default {
    name: 'film-detail',
    props: ['film']
}
</script>

<style>

</style>