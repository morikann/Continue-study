<template>
  <div>
    <v-row>
      <v-col>
        <h1 id='top-font' class="text-center mt-5">コンスタ</h1>
        <div class="mt-2">
          <p class="text-center font-weight-bold sub-title1"><span>環境・目標・習慣</span></p>
          <p class="text-center mt-1 sub-title2 ">この3つを身につけて勉強を継続させよう</p>
        </div>
      </v-col>
    </v-row>
    <v-row>
      <v-col class="text-center mt-10">
        <v-btn rounded color="light-blue lighten-3 mr-2" @click="toSignUp">
          新規登録
        </v-btn>
        <v-btn rounded color="cyan lighten-3 ml-2">
          ログイン
        </v-btn>
      </v-col>
    </v-row>
    <v-row>
      <v-col class="text-center mt-5">
        <v-btn color="orange lighten-3">
          かんたんログイン
        </v-btn>
      </v-col>
    </v-row>
  </div>
</template>

<script>

export default {
  data: function () {
    return {
      message: "Hello Vue!"
    }
  },
  methods: {
    toSignUp() {
      this.$router.push({ path: "signup" });
    },
  }
  // computed: {
  //   switch
  // }
}
</script>

<style scoped lang="scss">
@import 'reset-css';

$breakpoints: (
  'sm': 'screen and (min-width: 400px)',
  'md': 'screen and (min-width: 768px)',
  'lg': 'screen and (min-width: 1000px)',
  'xl': 'screen and (min-width: 1200px)',
) !default;

@mixin mq($breakpoint: md) {
  @media #{map-get($breakpoints, $breakpoint)} {
    @content;
  }
}

#top-font {
  font-size: 80px;
  font-family: 'top-font';

  @include mq() {
    font-size: 120px;
  }
}

.sub-title1 {
  font-size: 18px;

  @include mq() {
    font-size: 24px;
  }
}

.sub-title1 span {
  background: linear-gradient(transparent 70%, yellow 70%);
}

.sub-title2 {
  font-size: 16px;

  @include mq() {
    font-size: 20px;
  }
}

</style>

