<template>
  <v-row
    item-selector=".item"
  >
    <v-col
      v-for="movie in movies"
      :key="movie.imdbID"
      class="item"
      cols="12"
      lg="3"
      md="3"
      sm="6"
    >
      <nuxt-link :to="'/moviedetail/' + movie.imdbID">
        <v-card>
          <v-img
            :src="posterSrc(movie.Poster)"
            :alt="movie.Title"
            :height="posterHeight(movie.Poster)"
          >
            <template #placeholder>
              <div style="background: lightgray; height: 100%;" />
            </template>
          </v-img>
          <v-card-title>
            {{ movie.Title }}
          </v-card-title>
          <v-card-subtitle>
            {{ movie.Year }}
          </v-card-subtitle>
        </v-card>
      </nuxt-link>
    </v-col>
  </v-row>
</template>

<script>
import { mapState } from 'vuex';

export default {

    computed: {
      ...mapState('movie', ['movies']),
    },

  methods: {
    posterSrc (poster) {
      return poster === 'N/A' ? '' : poster
    },
    posterHeight (poster) {
      return poster === 'N/A' ? 100 : 300
    }
  }
}
</script>