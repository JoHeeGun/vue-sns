<template>
  <v-card style="margin-bottom: 20px">
    <v-container>
      <v-form ref="form" v-model="valid" @submit.prevent="onSubmitForm">
        <div>{{ me.nickname }}님 환영합니다!</div> <br>
        <v-textarea
          v-model="content"
          outlined
          auto-grow
          clearable
          label="어떤 영화에 대해 이야기 하고 싶으신가요?"
        />
        <v-btn type="submit" color="gray" absolute right>업로드</v-btn>
        <input ref="imageInput" type="file" multiple hidden @change="onChangeImages">
        <v-btn type="button" @click="onClickImageUpload">이미지 업로드</v-btn>
        <div>
          <div v-for="(p, i) in imagePaths" :key="p" style="display: inline-block">
            <img :src="`http://localhost:3085/${p}`" :alt="p" style="width: 200px">
            <div>
              <button type="button" @click="onRemoveImage(i)">제거</button>
            </div>
          </div>
        </div>
      </v-form>
    </v-container>
  </v-card>
</template>

<script>
  import { mapState } from 'vuex';
  export default {
    data() {
      return {
        valid: false,
        content: '',
      };
    },
    computed: {
      ...mapState('users', ['me']),
      ...mapState('posts', ['imagePaths'])
    },
    methods: {
      onSubmitForm() {
        if (this.$refs.form.validate()) {
          this.$store.dispatch('posts/add', {
            content: this.content,
          })
            .then(() => {
              this.content = '';
              this.hideDetails = false;
              this.success = true;
              this.successMessages = '게시글 등록 성공!';
            })
            .catch(() => {
            });
        }
      },
      onClickImageUpload() {
        this.$refs.imageInput.click();
      },
      onChangeImages(e) {
        console.log(e.target.files);
        const imageFormData = new FormData();
        [].forEach.call(e.target.files, (f) => {
          imageFormData.append('image', f);   
        });
        this.$store.dispatch('posts/uploadImages', imageFormData);
      },
      onRemoveImage(index) {
        this.$store.commit('posts/removeImagePath', index);
      }
    },
  };
</script>

<style>
</style>