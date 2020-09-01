<template>
  <v-theme-provider :dark="dark">
    <div>
      <base-info-card
        title="KEEP IN TOUCH WITH US"
        pace="6"
      >
        We are available 24/7

        <base-business-contact dense />
      </base-info-card>
    </div>
  </v-theme-provider>
</template>

<script>
  export default {
    name: 'BaseBusinessInfo',

    props: { dark: Boolean },

    data: () => ({
      business: [
        {
          icon: 'mdi-map-marker-outline',
          title: 'Address',
          text: 'Rue Sylvanie, Akwa',
        },
        {
          icon: 'mdi-cellphone',
          title: 'Phone',
          text: '+237 653 933 054<br>+237 655 659 721',
        },
        {
          icon: 'mdi-email',
          title: 'Email',
          text: 'burcoplus@yahoo.fr',
        },
      ],
    }),
  }
</script>
