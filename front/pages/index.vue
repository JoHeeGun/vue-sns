<template>
  <v-container>
    <v-carousel interval="1000">
      <v-carousel-item
        v-for="(item,i) in items"
        :key="i"
        :src="item.src"
      />
    </v-carousel><br>
    <post-form v-if="me" />
    <search-hash-tag />
    <div>
      <post-card v-for="p in mainPosts" :key="p.id" :post="p" />
    </div>
  </v-container>
</template>

<script>
  import PostCard from '~/components/PostCard';
  import PostForm from '~/components/PostForm';
  import SearchHashTag from '../components/SearchHashTag.vue';

  export default {
    components: {
      PostCard,
      PostForm,
      SearchHashTag,
    },
    data() {
      return {
        name: 'Nuxt.js',
        items: [
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg'
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg'
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg'
        },
        {
          src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg'
        }
      ]
      };
    },
    fetch({ store }) {
      return store.dispatch('posts/loadPosts', { reset: true });
    },
    computed: {
      me() {
        return this.$store.state.users.me;
      },
      mainPosts() {
        return this.$store.state.posts.mainPosts;
      },
      hasMorePost() {
        return this.$store.state.posts.hasMorePost;
      }
    },
    mounted() {
      window.addEventListener('scroll', this.onScroll);
    },
    beforeDestroy() {
      window.removeEventListener('scroll', this.onScroll);
    },
    methods: {
      onScroll() {
        console.log('scroll');
        if (window.scrollY + document.documentElement.clientHeight > document.documentElement.scrollHeight - 300) {
          if (this.hasMorePost) {
            this.$store.dispatch('posts/loadPosts');
          }
        }
      },
    },
  };
</script>

<style>

</style>