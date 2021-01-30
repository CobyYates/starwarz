<template>
  <!-- <v-container class="justify-center"> -->
    <v-row class="mb-12 mx-auto justify-center">
      <v-col v-for="item in cardData" :key="item.i" cols="6" sm="6" md="4" lg="3">
        <v-card height="300" width="auto" :elevation="$store.state.elevation">
          <v-img
            :src="`${item.image}`"
            height="100%"
          >
          <v-overlay absolute opacity=".2">
            <h3>{{ item.title }}</h3>
          </v-overlay>
          </v-img>
        </v-card>
      </v-col>
    </v-row>
  <!-- </v-container> -->
</template>

<script>
export default {
  name: "HomeCard",
  props: ["starship"],
  data: () => ({
    cardData: [
      {
        title: "People",
        image: "https://starwars-visualguide.com/assets/img/characters/1.jpg",
      },
      {
        title: "Films",
        image: "https://starwars-visualguide.com/assets/img/films/1.jpg",
      },
      {
        title: "Vehicles",
        image: "https://starwars-visualguide.com/assets/img/vehicles/6.jpg",
      },
      {
        title: "Starships",
        image: "https://starwars-visualguide.com/assets/img/starships/12.jpg",
      },
    ],
  }),
};
</script>
