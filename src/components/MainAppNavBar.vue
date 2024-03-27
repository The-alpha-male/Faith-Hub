<template>
  <v-app-bar :elevation="2">
    <template v-slot:prepend>
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
    </template>

    <v-app-bar-title>Application Bar</v-app-bar-title>
    <v-spacer> </v-spacer>

    <v-btn to="/" variant="outlined" size="large" rounded> home </v-btn>
    <v-spacer></v-spacer>
    <v-btn to="/about" variant="outlined" size="large" rounded> about us </v-btn>
    <v-btn to="/about" variant="outlined" size="large" rounded> Ourservices </v-btn>
    <v-btn to="/about" variant="outlined" size="large" rounded> contact </v-btn>
    <v-btn to="/about" variant="outlined" size="large" rounded> Blogs </v-btn>
  </v-app-bar>
</template>

<script setup></script>

<style lang="scss" scoped></style>
