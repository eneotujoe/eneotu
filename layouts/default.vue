<template>
  <v-app dark>
    <Navbar />
    <v-main class="secondary ma-2">
      <v-container>
        <nuxt />
      </v-container>
    </v-main>
    <Footer />
  </v-app>
</template>
<style>
html {
  background: #76ff03;
}
.v-application--wrap {
  background: #76ff03;
}
.v-main {
  align-items: center;
  height: 75%;
}
</style>
