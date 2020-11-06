<template>
  <div id="app">
    <v-app>
      <v-btn class="mx-2" fab dark large color="purple">
        <v-icon dark>
          mdi-android
        </v-icon>
      </v-btn>

      <v-icon large color="green darken-2">
        mdi-domain
      </v-icon>
    </v-app>
    <v-app>
      <v-btn class="mx-2" fab dark small color="pink">
        <v-icon>
          mdi-heart
        </v-icon>
      </v-btn>
    </v-app>

   

    <p>{{ message }}</p>
  </div>
</template>

<script>
export default {
  data: function () {
    return {
      message: "Hello Vue!"
    }
  }
}
</script>

<style scoped>
p {
  font-size: 2em;
  text-align: center;
}
</style>
