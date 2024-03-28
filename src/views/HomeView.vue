<template>
  <div class="container-fluid">
    <div class="hero-section d-flex justify-center align-center">
      <v-container class="d-flex">
        <v-card flat color="transparent" class="mx-auto ml-0" max-width="400">
          <v-card-title
            style="
              font-family: Sue Ellen Francisco;
              font-weight: 400;
              line-height: 54.15px;
              font-size: 50px;
            "
            class="text-white font-italic"
          >
            Need Help ....
          </v-card-title>
          <v-card-text>
            <p class="text-h4 text-white welcome-text">Being Life Saver For Someone</p>
          </v-card-text>
          <v-card-actions>
            <v-btn
              id="card-actionbtn"
              variant="outlined"
              rounded
              style="background-color: #ff6d6d; color: white"
            >
              Donate
            </v-btn>
            <v-btn
              id="card-actionbtn"
              variant="outlined"
              rounded
              style="background-color: #ffffff; color: #2e4049"
            >
              Discover
            </v-btn>
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
.welcome-text {
  font-family: 'Shippori Mincho';
  font-weight: 800;
  font-size: 90px;
  line-height: 57.47px;
}
#card-actionbtn {
  font-family: 'Work Sans';
  font-size: 18px;
  line-height: 21.11px;
  font-weight: 500;
}
</style>
