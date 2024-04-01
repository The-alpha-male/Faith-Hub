<template>
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
export default {
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
}
</script>
<style scoped>
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
