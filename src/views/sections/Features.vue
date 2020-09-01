<template>
  <base-section
    id="features"
    class="secondary"
  >
    <v-responsive
      class="mx-auto"
      max-width="1350"
    >
      <v-container fluid>
        <v-row>
          <v-col
            v-for="card in cards"
            :key="card.title"
            cols="12"
            sm="4"
            md="3"
          >
            <base-info-card
              align="center"
              dark
              v-bind="card"
 />
          </v-col>
        </v-row>
      </v-container>
    </v-responsive>
  </base-section>
</template>

<script>
/* eslint-disable */
  export default {
    name: 'SectionFeatures',

    data: () => ({
      cards: [
        {
          icon: 'mdi-keyboard-outline',
          title: 'Adaptability',
          text: 'We offer you an adaptation to each need with its multi-service, multi-company and multi-currency solutions',
        },
        {
          icon: 'mdi-pencil-outline',
          title: 'Realistic Objectives',
          text: " We are making history by focusing on achievable, long-term projects.",
        },
        {
          icon: 'mdi-camera-outline',
          title: 'Assurance',
          text: "Attention is focused on you and your various requirements. Live the moment fully with the firm conviction that your requests are taken care of.",
        },
        {
          icon: 'mdi-puzzle-outline',
          title: '24/7 Support',
          text: 'Your requests are handled 24/7 and a favorable response is offered to you promptly.',
        },
      ],
    }),
  }
</script>

