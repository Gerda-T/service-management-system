<template>
  <base-section id="presentation">
    <base-section-heading title="Presentation">
    Bureautic Company Plus is a multifunctional company whose goal is to satisfy its customers around the world by offering various services, business solutions specific to each individual according to his preferences. With its offers, Bureautic Company Plus responds to a specific need, at any time by offering the possibility of support for each service offered.
    </base-section-heading>

    <v-container>
      <v-row
          v-for="(feature,space, i) in features"
          :key="i"
          
          md="1"
        >
          <base-avatar-card
            v-bind="feature"
            align="right"
            horizontal
          >
          Bureautic Company Plus offers you fixed solutions to your requests: deliveries of computer materials, business solutions such as CMMS maintenance (Computer-assisted maintenance management) & After-sales service (After-sales service) which adapt to scope and orientation you want to give to your project, Oil expertise and study, Maintenance of IT tools and various services included in Industry and Buildings.
          </base-avatar-card>

        
      </v-row>
    </v-container>
  </base-section>
</template>

<script>
/* eslint-disable */
  export default {
    name: 'SectionThemeFeatures',

    data: () => ({
      features: [
        {
          title: ' MANAGEMENT, MAINTENANCE AND SERVICE PROPOSED BY BUREAUTIC COMPANY PLUS, S.A.R.L',
          color: '#050b1f !important',
          dark: true,
          icon: 'mdi-pencil-box-outline'
        },
       
      ],
    }),
  }
</script>
