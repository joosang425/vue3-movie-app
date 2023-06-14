<template>
  <Headline />
  <Search />
  <MovieList />
</template>

<script>
import Headline from '~/components/Haedline'
import Search from '~/components/Search.vue'
import MovieList from '../components/MovieList'

export default {
  components: {
    Headline,
    Search,
    MovieList
  },
  created() {
    this.$store.commit('movie/resetMovies')
  }
}
</script>