<template>
  <v-card max-width="500" class="mx-auto mt-10 px-5 pb-5">
    <v-card-title class="text-center">
      アカウント作成
    </v-card-title>
    <form>
      <v-text-field v-model="name" label="ユーザー名" required></v-text-field>
      <v-text-field v-model="email" label="メールアドレス"></v-text-field>
      <v-text-field v-model="password" label="パスワード" required></v-text-field>
      <v-text-field v-model="password_confirmation" label="パスワード確認" required></v-text-field>
      <v-select :items="items" label="都道府県"></v-select>
      <v-btn @click="submit">
        submit
      </v-btn>
    </form>
  </v-card>
</template>
 
<script>
  export default {
    data() {
      return {
        name: '',
        email: '',
        password: '',
        password_confirmation: '',
        select: null,
        items: [
          '北海道',
          '青森県',
          '岩手県',
          '宮城県',
          '秋田県',
          '山形県',
          '福島県',
          '茨城県',
          '栃木県',
          '群馬県',
          '埼玉県',
          '千葉県',
          '東京都',
          '神奈川県',
          '新潟県',
          '富山県',
          '石川県'
        ]
      }
    }
  }
</script>

<style scoped>

</style>