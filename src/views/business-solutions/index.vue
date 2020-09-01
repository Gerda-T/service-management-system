<script>
  // Extensions
  import View from '@/views/View'

  // Mixins
  import LoadSections from '@/mixins/load-sections'

  export default {
    name: 'Business Solutions',

    metaInfo: { title: 'Solution' },

    extends: View,

    mixins: [
      LoadSections([
        'Institutions',
        'Petroleum study and expertise',
        'Support and Purchase of DimoMaint Software',
        'IT Sector',
      ]),
    ],

    props: {
      id: {
        type: String,
        default: 'home',
      },
    },
  }
</script>
