<template>
  <footer class="container-flex">
    <div class="row">
      <FooterAbout />
      <FooterTweets />
      <FooterContacts :contacts="contacts"/>
      <FooterMap />


    </div>
  </footer>
</template>

<script>
import FooterAbout from './FooterAbout.vue'
import FooterTweets from './FooterTweets.vue'
import FooterContacts from './FooterContacts.vue'
import FooterMap from './FooterMap.vue'




export default {
  name: 'Footer',
  components: {
    FooterAbout,
    FooterTweets,
    FooterContacts,
    FooterMap,
    
    },
    data() {
      return {
        contacts: [
          {
            iconClass: 'fas fa-globe',
            text: 'Corporate location',
            address: '1600 Amphitheatre Parkway',
            postCode: 'London Wc11BA'
          },
          {
            iconClass: 'fas fa-home',
            text: 'Residential Location',
            address: '1600 Amphitheatre Parkway',
            postCode: 'London Wc11BA'
          },
          {
            iconClass: 'fas fa-phone',
            text: '1.800.458.556 / 1.800.532.2112',
          },
          {
            iconClass: 'fas fa-envelope',
            text: 'info@your-domain.com',
          },
          {
            iconClass: 'fas fa-clock',
            text: 'Monday - Friday: 9:00 AM - 6:00 PM',
          },
          {
            iconClass: 'fas fa-clock',
            text: 'Saturday - Sunday: 9:00 AM - 12:00 PM',
          },
        ]
      }
    }
}
</script>


<style lang="scss" scoped>
@import "../style/variables.scss";

footer {
  height: 500px;
}

</style>