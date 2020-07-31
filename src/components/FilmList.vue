<template>
  <div>
      <ul>
          <film-list-item v-for="(film, index) in films" :film="film" :key="index"></film-list-item>
      </ul>
  </div>
</template>

<script>
export default {
    name: 'film-list',
    props: ['films'],

}
</script>

<style>

</style>