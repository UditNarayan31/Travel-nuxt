<template>
  <v-card>
    <v-tabs
      v-model="tab"
      background-color="deep-purple accent-4"
      centered
      dark
      icons-and-text
    >
      <v-tabs-slider></v-tabs-slider>

      <v-tab href="#tab-1">
        Recents
        <v-icon>mdi-phone</v-icon>
      </v-tab>

      <v-tab href="#tab-2">
        Favorites
        <v-icon>mdi-heart</v-icon>
      </v-tab>

      <v-tab href="#tab-3">
        Nearby
        <v-icon>mdi-account-box</v-icon>
      </v-tab>
    </v-tabs>

    <v-tabs-items v-model="tab">
      <v-tab-item
       :value="'tab-1'"
      >
        <v-card flat>
          <v-card-text>1</v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>

      <v-tabs-items v-model="tab">
      <v-tab-item
       :value="'tab-2'"
      >
        <v-card flat>
          <v-card-text>2</v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>

      <v-tabs-items v-model="tab">
      <v-tab-item
       :value="'tab-3'"
      >
        <v-card flat>
          <v-card-text>3</v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs-items>

    
  </v-card>
</template>
<script>
  export default {
    data () {
      return {
        tab: null,
        text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.',
      }
    },
  }
</script>
