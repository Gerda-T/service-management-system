<template>
  <div>
    <v-tabs
      background-color="deep-blue accent-4"
      class="elevation-2"
      dark
      :centered="centered"
      :grow="grow"
      :vertical="vertical"
      :right="right"
      :prev-icon="prevIcon ? 'mdi-arrow-left-bold-box-outline' : undefined"
      :next-icon="nextIcon ? 'mdi-arrow-right-bold-box-outline' : undefined"
      :icons-and-text="icons"
    >
      <v-tab>
        <v-icon v-if="icons">
          mdi-phone
        </v-icon>
      </v-tab>
      <v-tab-item>
        <v-card
          flat
          tile
        >
          <v-card-text>{{ text }}</v-card-text>
        </v-card>
      </v-tab-item>

      <v-tab>
        <v-icon v-if="icons">
          mdi-phone
        </v-icon>
      </v-tab>
      <v-tab-item>
        <v-card
          flat
          tile
        >
          <v-card-text>{{ text }}</v-card-text>
        </v-card>
      </v-tab-item>

      <v-tab>
        <v-icon v-if="icons">
          mdi-phone
        </v-icon>
      </v-tab>
      <v-tab-item>
        <v-card
          flat
          tile
        >
          <v-card-text>{{ text }}</v-card-text>
        </v-card>
      </v-tab-item>
    </v-tabs>
  </div>
</template>

<script>
  /* eslint-disable */
  export default {
    data () {
      return {
        tab: null,
        text: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.',
        icons: true,
        centered: true,
        grow: true,
        vertical: false,
        prevIcon: false,
        nextIcon: false,
        right: false,
        tabs: 3,
      }
    },
  }
</script>

<style>
    .elevation-2{
        background-color: #050b1f !important;
    }
</style>