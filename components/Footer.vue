<template>
  <v-footer class="secondary">
    <v-row class="ma-5 success--text">
    <v-col cols="12" sm="12" md="3" class="text-center">
        <SocialLinks/>
      </v-col>
      <v-col class="my-5 text-center">
        <p>&copy; {{ new Date().getFullYear() }} - Eneotu Joe</p>
      </v-col>
    </v-row>
  </v-footer>
</template>
<style scoped>
.v-footer {
  height: 40%;
}
</style>
