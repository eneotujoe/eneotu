<template>
  <v-row>
    <v-navigation-drawer
      v-model="drawer"
      app
      absolute
      temporary
      dark
      class="secondary"
    >
      <v-list nav>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-content>
            <v-list-item-title class="success--text" v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar app flat height="7" class="success">
      <v-app-bar-nav-icon
        class="hidden-md-and-up secondary--text mt-5"
        dark
        @click.stop="drawer = !drawer"
      >
      </v-app-bar-nav-icon>
    </v-app-bar>
  </v-row>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
      items: [
        {
          title: 'Home',
          to: '/',
        },
        {
          title: 'About',
          to: '/about',
        },
        {
          title: 'Skills',
          to: '/skills',
        },
        {
          title: 'Projects',
          to: '/projects',
        },
      ],
    }
  },
}
</script>
