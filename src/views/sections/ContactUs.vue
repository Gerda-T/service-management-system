<!--template>
  <v-theme-provider dark>
    <base-section
      id="contact-us"
      class="black"
      space="40"
      
    >
      <v-container>
        <v-row justify="center">
          <v-col cols="10">
            <base-title
              :space="$vuetify.breakpoint.mdAndUp ? 0 : 4"
              title="DES QUESTIONS? NOUS LES RECEVONS!"
            />

            <base-body space="0">
              <span class="white--text">
                Posez-nous vos questions.
              </span>
            </base-body>
          </v-col>

          <v-col
            cols="12"
            md="2"
          >
            <base-btn
              :block="$vuetify.breakpoint.smAndDown"
              color="white"
              href="mailto:burcoplus@yahoo.fr"
              large
              outlined
              target="_blank"
            >
              Contactez-vous
            </base-btn>
          </v-col>
        </v-row>
      </v-container>
    </base-section>
  </v-theme-provider>
</template>

<script>
/* eslint-disable */
  export default {
    name: 'SectionContactUs',
  }
</script>
