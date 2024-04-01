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
  <div>
    <v-container>
      <v-row no-gutters>
        <v-col cols="4" class="no-space" v-for="carditem in inforCards" :key="carditem.color">
          <div
            :style="{
              width: '401px',
              height: '351px',
              backgroundColor: carditem.color,
              marginTop: '-100px',
              Padding: '67px, 40px, 68px, 40px'
            }"
            class="d-flex justify-center align-center"
          >
            <v-card color="transparent" flat height="216px" width="321px">
              <v-card-title class="mt-2 card-title">
                {{ carditem.title }}
              </v-card-title>
              <v-card-text>
                {{ carditem.content }}
              </v-card-text>
              <v-card-actions v-if="carditem.title === 'Education'">
                <v-btn class="" style="background-color: #ffffff" rounded size="large">
                  Discover
                </v-btn>
              </v-card-actions>
              <v-card-actions v-else>
                <a href="" style="color: #ffffff">JOIN ORGANIZATION</a>
              </v-card-actions>
            </v-card>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import { defineComponent } from 'vue'

// Components

export default defineComponent({
  name: 'HomeView',

  components: {},

  data: () => ({
    inforCards: [
      {
        color: '#77D7D3',
        title: 'Education',
        content:
          'Below Poverty Line is enchmark used by the government of India economic disadvantage.'
      },
      {
        color: '#2E4049',
        title: 'Become a Volunteer',
        content: 'Below Poverty Line is enchmark used by the government'
      },
      {
        color: 'white',
        title: '',
        content: ''
      }
    ]
  })
})
</script>
<style scoped>
.container-fluid {
  background-image: url('/src/assets/homeimage.jpeg');
  height: 920px;
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
.hero-section {
  background: linear-gradient(103.5deg, rgba(19, 35, 45, 0.69) 3.46%, rgba(29, 39, 45, 0) 51.8%);
  height: 920px;
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
.no-space {
  padding: 0 !important;
  margin: 0 !important;
}
.card-title {
  font-family: 'Shippori Mincho';
  font-size: 35px;
  font-weight: 800;
  line-height: 37.9px;
  text-align: left;
}
</style>
