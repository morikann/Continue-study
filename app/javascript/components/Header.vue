<template>
  <div>
    <v-app-bar color="blue lighten-3">
      <v-toolbar-title class="font-weight-bold">コンスタ</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>
    </v-app-bar>
  </div>
</template>

<script>

export default {
  data: function () {
    return {
      message: "Hello Vue!"
    }
  },
  // computed: {
  //   switch
  // }
}
</script>

<style scoped lang="scss">
