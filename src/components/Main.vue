<template>
   <main>
       <Jumbotron />
       <ConstructionProjectsTop />
       <ConstructionProjectsBottom />
       <Statistics />
       <RecentWork />


   </main>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import ConstructionProjectsTop from './ConstructionProjectsTop.vue'
import ConstructionProjectsBottom from './ConstructionProjectsBottom.vue'
import Statistics from './Statistics.vue'
import RecentWork from './RecentWork.vue'




export default {
  name: 'Main',
  components: {
      Jumbotron,
      ConstructionProjectsTop,
      ConstructionProjectsBottom,
      Statistics,
      RecentWork
  }
}
</script>


<style lang="scss" scoped>
@import "../style/variables.scss";


</style>