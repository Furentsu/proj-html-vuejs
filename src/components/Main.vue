<template>
   <main>
       <Jumbotron />
       <ConstructionProjectsTop />
       <ConstructionProjectsBottom />

   </main>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import ConstructionProjectsTop from './ConstructionProjectsTop.vue'
import ConstructionProjectsBottom from './ConstructionProjectsBottom.vue'


export default {
  name: 'Main',
  components: {
      Jumbotron,
      ConstructionProjectsTop,
      ConstructionProjectsBottom
  }
}
</script>


<style lang="scss" scoped>
@import "../style/variables.scss";


</style>