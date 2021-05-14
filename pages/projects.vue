<template>
  <v-row class="primary--text ma-5">
      <h1>Projects</h1>   
    <v-col
      v-for="(link, i) in links"
      :key="i"
      cols="12"
      md="12"
    >  
      <v-btn
        text
        class="primary--text text-capitalize"
        :href="link.url"
      >
        {{ link.text }}
      </v-btn>
    </v-col>
  </v-row>
</template>
<script>
export default {
  data() {
    return{
      links: [
        {url:'https://netflix-pro.netlify.app', text: 'Netflix Frontend Clone: Built With ReactJS'},
        {url:'https://instagram-pro.netlify.app', text: 'Instagram Frontend Clone: Built With ReactJS'},
        {url:'https://eneotu.netlify.app', text: 'My Portfolio'},
        {url:'https://preptask.netlify.app/quiz', text: 'Preptask: an educational tool built with nuxt, Django and GraphQL'},
        {url:'https://event-nigeria.netlify.app/', text: 'Event Nigeria: an event app built with nuxt, strapi and GraphQL'},
      ]
    }
  }
}
</script>