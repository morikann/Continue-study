<template>
  <v-app>
    <v-container>
      <router-view></router-view>
    </v-container>
  </v-app>
</template>

<script>
import Vue from 'vue';
import VueRouter from 'vue-router';

import HomePage from './HomePage.vue';

const router = new VueRouter({
  // mode: 'history',
  routes: [
    { path: '/', component: HomePage }
  ]
})

Vue.use(VueRouter)

export default {
  router
}
</script>

<style scoped>

</style>
