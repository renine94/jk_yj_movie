<template>
  <div class="card col-12 col-sm-6 col-lg-3" style="width: 18rem;">
    <img :src="movie.poster_url" class="card-img-top" alt="Movie Poster">
    <div class="card-body">
      <h5 class="card-title">{{ movie.title }}</h5>
      <MovieListItemModal :movie="movie"/>
    </div>
  </div>

</template>

<script>
import MovieListItemModal from '../components/MovieListItemModal'

export default {
  name:'MovieListItem',
  components: {
    MovieListItemModal,
  },
  props:{
    movie: Object,
  },
}
</script>

<style>

</style>
