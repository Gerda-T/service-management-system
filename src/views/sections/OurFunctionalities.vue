<template>
  <base-section id="our-functionalities">
    <base-section-heading
      color="#050b1f !important"
      title="Our Functionalities"
    />

    <v-container>
      <v-row>
        <v-col
          v-for="card in cards"
          :key="card.title"
          cols="12"
          md="4"
        >
          <base-info-card v-bind="card" />
        </v-col>
      </v-row>
    </v-container>
  </base-section>
</template>

<script>
  export default {
    name: 'SectionOurFunctionalities',

    data: () => ({
      cards: [
        {
          title: 'Management and Maintenance',
          text: 'The services management offerred by BUREAUTIC COMPANY PLUS assures un follow-up,Organization of equipments,Technical description,Life cycle management, A traceability of changes over time, Management of stock purchased and Customer management',
        },
        {
          title: 'After Sales Service', 
          text: 'After sales services assures a follow up of every service delvered by us or not, Management of requests and calls, interventions, Contract management and After sales reports, Tools for for monitoring maintenance, and a financial management tool for monitoring cost.',
          
        },
        {
          title: 'Benefits',
          text: 'BUREAUTIC COMPANY PLUS aims at providing efficient solutions to various business solutions, Efficient service management and maintenance. Efficient maintenance allows better return on investment and avoids critical breakdowns, generating late deliveries or service disruptions.',
        },
      ],
    }),
  }
</script>
