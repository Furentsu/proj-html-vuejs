<template>
  <div class="col-3">
      <h3>Find us</h3>

      <div class="img-container">
         <img src="../assets/images/construction_map_pin.png" alt="Company's location">
      </div>
      
  </div>
</template>

<script>
export default {
    name: 'FooterMap',
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

h3 {
    color: $vibrantBrightSun;
    font-size: 1.2rem;
    padding-bottom: 20px;
}

.img-container {
    border: 1px solid white;

    img {
        width: 100%;
    }
}

</style>