<template>
  <footer class="container-flex">
    <div class="row">
      <FooterAbout />

    </div>
  </footer>
</template>

<script>
import FooterAbout from './FooterAbout.vue'

export default {
  name: 'Footer',
  components: {
    FooterAbout
    }
}
</script>


<style lang="scss" scoped>
@import "../style/variables.scss";

footer {
  height: 500px;
}

</style>