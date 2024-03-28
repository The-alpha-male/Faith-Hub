<template>
  <div class="container-fluid">
    <div class="hero-section d-flex justify-center align-center">
      <v-container class="d-flex">
        <v-card flat color="transparent" class="mx-auto ml-0" max-width="344">
          <v-card-text>
            <div>Word of the Day</div>
            <p class="text-h4 text--primary">be•nev•o•lent</p>
            <p>adjective</p>
            <div class="text--primary">
              well meaning and kindly.<br />
              "a benevolent smile"
            </div>
          </v-card-text>
          <v-card-actions>
            <v-btn color="deep-purple-accent-4" variant="text"> Learn More </v-btn>
          </v-card-actions>
        </v-card>
      </v-container>
    </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue'

// Components

export default defineComponent({
  name: 'HomeView',

  components: {}
})
</script>
<style scoped>
.container-fluid {
  background-image: url('/src/assets/homeimage.jpeg');
  height: 100%;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
.hero-section {
  background: linear-gradient(103.5deg, rgba(19, 35, 45, 0.69) 3.46%, rgba(29, 39, 45, 0) 51.8%);
  height: 970px;
}
</style>
