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
      <v-system-bar height="50">
        <v-btn to='/' block tile text class="primary--text">eneotu</v-btn>
      </v-system-bar>
      <v-list nav>
        <v-list-item>
          <v-list-item-title class="primary--text"><v-btn to='/about' block tile text class="primary--text">About</v-btn></v-list-item-title>
        </v-list-item>
        <v-list-item>
          <v-list-item-title class="primary--text"><v-btn href='/resume.pdf' block tile text class="primary--text">Resume</v-btn></v-list-item-title>
        </v-list-item>
        <v-list-item>
          <v-list-item-title class="primary--text"><v-btn to='/project' block tile text class="primary--text">Project</v-btn></v-list-item-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar app flat height="15" class="secondary">
      <v-app-bar-nav-icon
        class="hidden-md-and-up primary--text ml-n7"
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
    }
  },
}
</script>
