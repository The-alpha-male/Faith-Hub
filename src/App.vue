<template>
  <v-app>
    <v-main>
      <main-app-nav-bar />
      <router-view />
    </v-main>
  </v-app>
</template>

<script>
import MainAppNavBar from './components/MainAppNavBar.vue'

export default {
  name: 'App',
  components: {
    MainAppNavBar
  },

  data: () => ({
    //
  })
}
</script>
