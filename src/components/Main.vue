<template>
   <main>
       <Jumbotron />
       <ConstructionProjectsTop />
       <ConstructionProjectsBottom />
       <Statistics />
       <RecentWork />
       <CoreValues />
       <Slider />
       <LatestNews />
       <TrustedPartners />
       <FinalJumbotron />
   </main>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import ConstructionProjectsTop from './ConstructionProjectsTop.vue'
import ConstructionProjectsBottom from './ConstructionProjectsBottom.vue'
import Statistics from './Statistics.vue'
import RecentWork from './RecentWork.vue'
import CoreValues from './CoreValues.vue'
import Slider from './Slider.vue'
import LatestNews from './LatestNews.vue'
import TrustedPartners from './TrustedPartners.vue'
import FinalJumbotron from './FinalJumbotron.vue'





export default {
  name: 'Main',
  components: {
      Jumbotron,
      ConstructionProjectsTop,
      ConstructionProjectsBottom,
      Statistics,
      RecentWork,
      CoreValues,
      Slider,
      LatestNews,
      TrustedPartners,
      FinalJumbotron
  }
}
</script>


<style lang="scss" scoped>
@import "../style/variables.scss";


</style>