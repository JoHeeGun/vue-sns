<template>
  <div v-if="me">
    <div>
      <v-container>
        <v-card style="margin-bottom: 20px">
          <v-container>
            {{ me.nickname }}님의 프로필입니다
            <v-row>
              <v-col cols="4">{{ me.Followings.length }} 팔로잉</v-col>
              <v-col cols="4">{{ me.Followers.length }} 팔로워</v-col>
              <v-col cols="4">{{ me.Posts.length }} 게시글</v-col>
            </v-row>
          </v-container>
        </v-card>
      
        <v-card style="margin-bottom: 20px">
          <v-container>
            <v-subheader>내 프로필</v-subheader>
            <v-form v-model="valid" @submit.prevent="onChangeNickname">
              <v-text-field
                v-model="nickname"
                label="변경할 닉네임을 적어주세요!"
                :rules="nicknameRules"
                required
              />
              <v-btn dark color="gray" type="submit">수정</v-btn>
            </v-form>
          </v-container>
        </v-card>
     
      

        <v-card style="margin-bottom: 20px">
          <v-container>
            <v-subheader>팔로잉</v-subheader>
            <follow-list :users="followingList" :remove="removeFollowing" />
            <v-btn v-if="hasMoreFollowing" dark color="blue" style="width: 100%" @click="loadMoreFollowings">더보기</v-btn>
          </v-container>
        </v-card>
        <v-card style="margin-bottom: 20px">
          <v-container>
            <v-subheader>팔로워</v-subheader>
            <follow-list :users="followerList" :remove="removeFollower" />
            <v-btn v-if="hasMoreFollower" dark color="blue" style="width: 100%" @click="loadMoreFollowers">더보기</v-btn>
          </v-container>
        </v-card>
      </v-container>
    </div>
  </div>
</template>

<script>
  import { mapState } from 'vuex';
  import FollowList from '~/components/sns/FollowList';

  export default {
    components: {
      FollowList,
    },
    middleware: 'authenticated',
    data() {
      return {
        valid: false,
        nickname: '',
        nicknameRules: [
          v => !!v || '닉네임을 입력하세요.',
        ],
      };
    },
    fetch({ store }) {
      return Promise.all([
        store.dispatch('users/loadFollowings', { offset: 0 }),
        store.dispatch('users/loadFollowers', { offset: 0 }),
      ]);
    },
    head() {
      return {
        title: '프로필',
      };
    },
    computed: {
      ...mapState('users', ['me','followerList','followingList','hasMoreFollowing','hasMoreFollower']),
    },
    methods: {
      onChangeNickname() {
        this.$store.dispatch('users/changeNickname', {
          nickname: this.nickname,
        });
      },
      removeFollowing(userId) {
        this.$store.dispatch('users/unfollow', { userId });
      },
      removeFollower(userId) {
        this.$store.dispatch('users/removeFollower', { userId });
      },
      loadMoreFollowers() {
        this.$store.dispatch('users/loadFollowers');
      },
      loadMoreFollowings() {
        this.$store.dispatch('users/loadFollowings');
      },
    },
  };
</script>

<style>
</style>