<template>
  <v-app dark>
    <Navbar />
    <v-main class="primary">
      <v-card min-height="70vh" class="secondary ma-5">
        <nuxt />
      </v-card>
    </v-main>
    <Footer />
  </v-app>
</template>
<style>
html {
  background: #76ff03;
}
</style>
