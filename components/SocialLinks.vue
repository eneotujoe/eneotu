<template>
    <v-row class="primary--text">
      <v-col cols="12" class="text-center">
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
    </v-row>
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
