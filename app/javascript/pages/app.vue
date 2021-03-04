<template>
  <v-app color="primary">
    <Header></Header>
    <v-main>
      <v-container fluid>
        <router-view></router-view>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import Vue from 'vue';
import VueRouter from 'vue-router';

import HomePage from './HomePage.vue';
import Header from '../components/Header';
import SignUp from './SingUp';

const router = new VueRouter({
  mode: 'history',
  routes: [
    { path: '/', component: HomePage },
    { path: '/signup', component: SignUp }
  ]
})

Vue.use(VueRouter)

export default {
  components: { Header },
  router
}
</script>

<style scoped>

</style>
