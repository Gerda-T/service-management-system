<script>
/* eslint-disable */
  // Extensions
  import View from '@/views/View'

  // Mixins
  import LoadSections from '@/mixins/load-sections'

  export default {
    name: 'ServiceDeliveries',

    metaInfo: { title: 'Service Deliveries' },

    extends: View,

    mixins: [
      LoadSections([
        'service-deliveries',
        
      ]),
    ],

    props: {
      id: {
        type: String,
        default: 'about',
      },
    },
  }
</script>
