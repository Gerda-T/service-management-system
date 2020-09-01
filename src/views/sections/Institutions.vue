<template>
<base-section>
<base-section-heading title="Institutions">
    Bureautic Company Plus offers sercices in institutions such as deliveries or post follow up services. Deliveries made includes:<br>deliveries of computers <br>photocopiers<br> inks<br> printers<br> automatic document feeders<br> color drum own by our partners all over the Country.<br>
    
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


</base-section>
    





</template>