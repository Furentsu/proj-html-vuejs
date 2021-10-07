<template>
   <main>
       <Jumbotron />
       <ConstructionProjectsTop />
       <ConstructionProjectsBottom />
       <Statistics />
       <RecentWork />
       <CoreValues />
       <!-- <Slider /> -->
       <LatestNews />
       <TrustedPartners />




   </main>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import ConstructionProjectsTop from './ConstructionProjectsTop.vue'
import ConstructionProjectsBottom from './ConstructionProjectsBottom.vue'
import Statistics from './Statistics.vue'
import RecentWork from './RecentWork.vue'
import CoreValues from './CoreValues.vue'
// Slider
import LatestNews from './LatestNews.vue'
import TrustedPartners from './TrustedPartners.vue'




export default {
  name: 'Main',
  components: {
      Jumbotron,
      ConstructionProjectsTop,
      ConstructionProjectsBottom,
      Statistics,
      RecentWork,
      CoreValues,
      // Slider,
      LatestNews,
      TrustedPartners
  }
}
</script>


<style lang="scss" scoped>
@import "../style/variables.scss";


</style>