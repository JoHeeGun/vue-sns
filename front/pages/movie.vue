<template>
  <v-app>
    <v-container class="pt-10">
      <search-bar />
      <movie-list />
    </v-container>
  </v-app>
</template>

<script>
import SearchBar from '../components/movie/SearchBar.vue'
import MovieList from '../components/movie/MovieList.vue'

export default {
components:{
  SearchBar,
  MovieList
}
}
</script>

<style>

</style>