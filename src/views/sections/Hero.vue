<template>
  <section id="hero">
    <v-img
      :min-height="minHeight"
      :src="require('@/assets/home-hero.jpg')"
      class="white--text"
      gradient="to right, rgba(5, 11, 31, .8), rgba(5, 11, 31, .8)"
    >
      <v-container class="fill-height px-4 py-12">
        <v-responsive
          class="d-flex align-center"
          height="100%"
          max-width="700"
          width="100%"
        >
          <base-heading title=" A SOLUTION TO EVERY QUESTION" />

          <base-body>
             Whatever the size of your requests, whatever your location, BUREAUTIC COMPANY Plus S.A.R.L assures you a complete education, a real solution and an adequate follow-up of your various requirements.
          </base-body>
        </v-responsive>
      </v-container>
    </v-img>
  </section>
</template>

<script>
 /* eslint-disable */
  export default {
    name: 'SectionHero',

    provide: {
      theme: { isDark: true },
    },

    computed: {
      minHeight () {
        const height = this.$vuetify.breakpoint.mdAndUp ? '100vh' : '50vh'

        return `calc(${height} - ${this.$vuetify.application.top}px)`
      },
    },
  }
</script>
