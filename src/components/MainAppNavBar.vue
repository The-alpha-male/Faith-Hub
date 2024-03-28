<template>
  <v-system-bar height="50" color="#77D7D3">
    <v-container height="50" class="d-flex">
      <div class="d-flex p-auto">
        <v-text class="px-4 text-subtitle-1 text-#126360">
          <v-icon class="pa-2" size="small"> mdi-phone </v-icon>
          +2547256798
        </v-text>
        <p>
          <v-icon class="px-2" size="small" color="#126360"> mdi-email </v-icon>
          munenronny@gmail.com
        </p>
      </div>
      <v-spacer></v-spacer>
      <div>
        <v-icon size="x-large" class="px-6" color="#126360"> mdi-instagram </v-icon>
        <v-icon size="x-large" class="px-6" color="#126360"> mdi-facebook </v-icon>
        <v-icon size="x-large" class="px-6" color="#126360"> mdi-twitter </v-icon>
        <v-icon size="x-large" class="px-6" color="#126360"> mdi-youtube </v-icon>
      </div>
    </v-container>
  </v-system-bar>
  <v-app-bar :elevation="0" app height="64">
    <!-- <template v-slot:prepend>
      <v-app-bar-nav-icon></v-app-bar-nav-icon>
    </template>

    <v-app-bar-title>Application Bar</v-app-bar-title> -->
    <v-img contain src="/src/assets/faith.png" max-height="125" class="ml-16" tile> </v-img>
    <v-spacer></v-spacer>
    <v-row no-gutters class="pa-14">
      <v-col cols="auto" class="">
        <v-btn to="/" variant="text"> home </v-btn>
      </v-col>
      <v-col cols="auto">
        <v-btn to="/about" variant="text"> about us </v-btn>
      </v-col>
      <v-col cols="auto">
        <v-btn to="" variant="text"> Ourservices </v-btn>
      </v-col>
      <v-col cols="auto">
        <v-btn to="" variant="text"> contact </v-btn>
      </v-col>
      <v-col cols="auto">
        <v-btn to="" variant="text"> Blogs </v-btn>
      </v-col>
      <v-col cols="auto">
        <v-btn color="#FF6D6D" rounded="xl" size="large" bloc to="" variant="flat"> donate </v-btn>
      </v-col>
    </v-row>
  </v-app-bar>
</template>

<script setup></script>

<style lang="scss" scoped></style>
