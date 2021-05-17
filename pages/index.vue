<template>
  <v-container>
    <v-row justify="center" align="center" class="primary--text mt-3">
      <v-col cols="12" sm="12" md="3" class="text-center">
        <h1 class="text-no-wrap">Eneotu Joe</h1>
        <p class="font-weight-thin">Software Engineer</p>
        <v-btn to="/contact" nuxt outlined class="primary--text">
          Contact Me
        </v-btn>
      </v-col>
      <v-col cols="12" sm="12" md="6" class="text-center mb-3">
        <v-img
          :src="require('../assets/photo.png')"
          alt="photo"
          height="200"
          eager
          contain
        />
      </v-col>
      <v-col>
        <v-col cols="12" sm="12" md="3" class="text-center">
          <v-btn
            v-for="(link, i) in links"
            :key="i"
            :href="link.url"
            outlined
            fab
            small
            class="ma-1 primary--text"
            icon
            target="_blank"
          >
            <v-icon size="20">
              {{ link.icon }}
            </v-icon>
          </v-btn>
        </v-col>
      </v-col>
    </v-row>
    <v-row justify="center" align="center">
      <v-col cols="12" class="text-center">
        <v-btn to="/about" outlined class="primary--text mb-1">About</v-btn>
        <v-btn href="/resume.pdf" outlined class="primary--text mb-1">Resume</v-btn>
        <v-btn to="/projects" outlined class="primary--text mb-1">
          Projects
        </v-btn>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    links: [
      {
        icon: 'mdi-twitter',
        url: 'https://twitter.com/eneotujoe',
      },
      {
        icon: 'mdi-linkedin',
        url: 'https://www.linkedin.com/in/eneotujoe/',
      },
      {
        icon: 'mdi-github',
        url: 'https://github.com/eneotujoe',
      },
    ],
  }),
}
</script>
<style scoped>
h1 {
  /* font-size: 6rem; */
  font-weight: lighter;
  text-transform: uppercase;
}
</style>
