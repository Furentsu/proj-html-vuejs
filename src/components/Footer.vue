<template>
  <footer class="container-flex">
    <div class="row">
      <FooterAbout />
      <FooterTweets />


    </div>
  </footer>
</template>

<script>
import FooterAbout from './FooterAbout.vue'
import FooterTweets from './FooterTweets.vue'


export default {
  name: 'Footer',
  components: {
    FooterAbout,
    FooterTweets,
    
    }
}
</script>


<style lang="scss" scoped>
@import "../style/variables.scss";

footer {
  height: 500px;
}

</style>