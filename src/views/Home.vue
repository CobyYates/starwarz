<template>
  <v-container class="fluid mx-0 px-0">
    <v-row class="mx-0 px-0">
      <v-col cols="12" class="mx-0 px-0">
        <v-parallax
          src="https://media.contentapi.ea.com/content/dam/eacom/en-us/migrated-images/2016/11/home-page-gohtrailer-desktop.jpg.adapt.crop16x9.1920w.jpg"
          class="d-flex justify-center headline-2 par"
        >
          <h1>Star Wars API</h1>
        </v-parallax>
      </v-col>
    </v-row>
    <v-row class="justify-center">
      <HomeCard class="justify-center" />
      <!-- <v-col v-for="item in $store.state.starships"
      :key="item.i"
      cols="3"
      >
        <Card :starship="item" />
      </v-col> -->
    </v-row>
  </v-container>
</template>

<script>
import HomeCard from '../components/HomeCards'

export default {
  name: "Home",
  components: {
    HomeCard
  }
};
</script>

<style scoped>
.par {
  width: 100vw;
}
</style>