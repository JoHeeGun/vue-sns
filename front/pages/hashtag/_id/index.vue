<template>
  <v-container>
    <div>
      <post-card v-for="p in mainPosts" :key="p.id" :post="p" />
    </div>
  </v-container>
</template>

<script>
  import PostCard from '~/components/sns/PostCard';
  import { mapState } from 'vuex'
  export default {
    components: {
      PostCard,
    },
    data() {
      return {
        name: 'Nuxt.js',
      };
    },
    fetch({ store, params }) {
      return store.dispatch('posts/loadHashtagPosts', {
        hashtag: encodeURIComponent(params.id),
        reset: true,
      });
    },
    computed: {
      ...mapState('posts', ['mainPosts'])
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