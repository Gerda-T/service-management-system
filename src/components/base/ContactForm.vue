<template>
  <div>
    <base-info-card
      :title="title"
      :subtitle="subtitle"
      space="4"
      color="primary"
    />

    <base-text-field label="Name" />

    <base-text-field label="Email" />

    <base-text-field label="Subject" />

    <base-textarea
      class="mb-6"
      label="Your need & Description"
    />

    <base-btn
      :color="!theme.isDark ? 'accent' : 'white'"
      href="mailto:burcoplus@yahoo.fr"
      outlined
      target="_blank"
    >
      SEND
    </base-btn>
  </div>
</template>

<script>
  export default {
    name: 'BaseContactForm',

    // Injected from the Vuetify Themeable mixin
    inject: ['theme'],

    props: {
      subtitle: String,
      title: {
        type: String,
        default: 'MAKE A REQUEST',
      },
    },
  }
</script>
