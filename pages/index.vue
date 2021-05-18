<template>
  <v-row justify="center" align="center" class="primary--text">
    <v-col cols="12" sm="12" md="4" class="text-center">
      <h1 class="text-no-wrap">Eneotu Joe</h1>
      <p class="font-weight-thin">Software Engineer</p>
      <v-btn to="/contact" nuxt outlined class="primary--text">
        Contact Me
      </v-btn>
    </v-col>
    <v-col cols="12" sm="12" md="4" class="text-center">
      <v-img
        :src="require('../assets/photo.png')"
        alt="photo"
        height="200"
        eager
        contain
      />
    </v-col>
      <v-col cols="12" sm="12" md="4" class="text-center">
        <v-btn to="/about" outlined class="primary--text mb-1">About</v-btn>
        <v-btn href="/resume.pdf" width="80" outlined class="primary--text mb-1">Resume</v-btn>
        <v-btn to="/project" width="80" outlined class="primary--text mb-1">Project</v-btn>
      </v-col>
  </v-row>
</template>

<script>
export default {
  
}
</script>
<style scoped>
h1 {
  /* font-size: 6rem; */
  font-weight: lighter;
  text-transform: uppercase;
}
/* .v-image {
  border: 1px solid #76FF03;
  border-radius: 50%;
} */
/* .v-btn:hover {
  background-color: #76ff03;
  color: #000000;
  opacity: unset;
} */
</style>
