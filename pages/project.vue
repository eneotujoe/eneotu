<template>
  <v-row class="primary--text ma-5">
    <h2 class="ml-3">Projects</h2>   
    <v-col
      v-for="(link, i) in links"
      :key="i"
      cols="12"
      md="12"
    >  
      <a
        text
        class="primary--text text-capitalize"
        :href="link.url"
      >
        {{ link.text }}
      </a>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data() {
    return{
      links: [
        {url:'https://netflix-pro.netlify.app', text: 'Netflix Frontend Clone: Built With ReactJS and deployed on netlify'},
        {url:'https://instagram-pro.netlify.app', text: 'Instagram Frontend Clone: Built With ReactJS and netlify'},
        {url:'https://eneotu.netlify.app', text: 'My Portfolio: built with nuxt and netlify'},
        {url:'https://preptask.netlify.app/quiz', text: 'Preptask: an educational tool built with nuxt, Django, GraphQL, heroku and netlify'},
        {url:'https://event-nigeria.netlify.app/', text: 'EventApp: an event schedule app built with nuxt, strapi, GraphQL, heroku and netlify'},
        {url:'https://blog-pro-1.netlify.app/', text: 'Blog: Built with nuxt, strapi, GraphQL, heroku and netlify'},
      ]
    }
  }
}
</script>
<style scoped>
a {
  text-decoration: none;
}
a:after {
  content: "";
  position: absolute;
  background-color:#76FF03;
  height: 1rem;
  width: 0;
  left: 3rem;
  top: 1px;
  transition: 0.3s;
}

a:hover:after {
  width: 80%;
}
</style>
