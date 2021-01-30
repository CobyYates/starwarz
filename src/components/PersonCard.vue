<template>
<v-container>
    <v-card
      height="300"
    >
      <!-- <v-img :src="`${item.image}`" /> -->
      {{starship.name}}
    </v-card>
</v-container>
</template>

<script>
export default {
  name: "HomeCard",
  props: ["starship"],
  data: () => ({
  })
};
</script>
