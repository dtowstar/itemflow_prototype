<template>
  <v-layout row class="pd-5">
    <v-flex xs12 sm6 offset-sm2 class="pt-5">
      <v-card>
        <v-flex xs12>
          <v-img
            src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
            width="300px"
            style="float: left;"
          ></v-img>
          <v-text-field v-model="first" label="First Name" box></v-text-field>
        </v-flex>

        <v-card-actions>
          <v-btn flat>Share</v-btn>
          <v-btn flat color="purple">Explore</v-btn>
          <v-spacer></v-spacer>
          <v-btn icon @click="show = !show">
            <v-icon>{{ show ? 'keyboard_arrow_down' : 'keyboard_arrow_up' }}</v-icon>
          </v-btn>
        </v-card-actions>

        <v-slide-y-transition>
          <v-card-text
            v-show="show"
          >I'm a thing. But, like most politicians, he promised more than he could deliver. You won't have time for sleeping, soldier, not with all the bed making you'll be doing. Then we'll go with that data file! Hey, you add a one and two zeros to that or we walk! You're going to do his laundry? I've got to find a way to escape.</v-card-text>
        </v-slide-y-transition>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  name: "CreateItemFlow",
  data: () => ({
    cards: [
      {
        title: "Pre-fab homes",
        src: "https://cdn.vuetifyjs.com/images/cards/house.jpg",
        flex: 12
      },
      {
        title: "Pre-fab homes",
        src: "https://cdn.vuetifyjs.com/images/cards/house.jpg",
        flex: 12
      }
    ]
  })
};
</script>

<style>
</style>
