<template>
  <v-list>
    <v-col v-for="user in users" :key="user.id" cols="12" md="4" style="display: inline-block">
      <v-list-item>
        <v-card-title>
          <h3>
            <nuxt-link :to="'/user/' + user.id">{{ user.nickname[0] }}</nuxt-link>
          </h3>
        </v-card-title>

        <v-list-item-content>
          <v-list-item-title>{{ user.nickname }}</v-list-item-title>
        </v-list-item-content>
        <v-list-item-action>
          <v-icon @click="remove(user.id)">mdi-minus-circle-outline</v-icon>
        </v-list-item-action>
      </v-list-item>
    </v-col>
  </v-list>
</template>

<script>
  export default {
    props: {
      abc: Array,
      users: {
        type: Array,
        required: true,
      },
      remove: {
        type: Function,
        required: true,
      }
    },
  }
</script>

<style>
</style>