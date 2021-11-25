<template>
  <v-form v-if="me" ref="form" v-model="valid" style="position: relative" @submit.prevent="onSubmitForm">
    <v-textarea
      v-model="content"
      filled
      auto-grow
      label="댓글 달기"
    />
    <v-btn color="gray" dark absolute top right type="submit">작성</v-btn>
  </v-form>
</template>

<script>
  export default {
    props: {
      postId: {
        type: Number,
        required: true,
      },
    },
    data() {
      return {
        valid: false,
        content: '',
      };
    },
    computed: {
      me() {
        return this.$store.state.users.me;
      },
    },
    methods: {
      onSubmitForm() {
        if (this.$refs.form.validate()) {
          this.$store.dispatch('posts/addComment', {
            postId: this.postId,
            content: this.content,
          })
            .then(() => {
              this.content = '';
            })
            .catch(() => {
            });
        }
      },
    },
  };
</script>

<style>
</style>