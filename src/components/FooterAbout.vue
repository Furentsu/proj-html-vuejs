<template>
  <div class="col-3">
      <div class="logo-container">
         <img src="../assets/images/footer-logo.png" alt="Avada Construction">
      </div>
      
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Error deserunt incidunt minus aliquam molestias nobis, natus laborum nam autem odit aliquid impedit soluta facere unde est praesentium numquam asperiores voluptatum?</p>
      <button>Learn More</button>  
  </div>
</template>

<script>
export default {
    name: 'FooterAbout',
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

.logo-container {
    img {
        width: 180px;
    }
}

p {
    color: $doveGrey;
    padding: 25px 0 10px 0;
}

button {
    border: 2px solid transparent;
    padding: 10px 50px;
    background-color: $vibrantBrightSun;
    color: $doveGrey;

    &:hover {
        border: 2px solid $primaryWhite;
        color: $primaryWhite;
    }
}

</style>