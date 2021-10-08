<template>
  <footer class="container-flex">
    <div class="row">
      <div class="col-8 left-content">
        <p>copyright 2012 - 2015 avada theme by <span> theme fusion</span> | all rights reserved | powered by <span> wordpress</span></p>
      </div>
      <div class="col-4 right-content">
        <i class="fab fa-facebook-f"></i>
        <i class="fab fa-twitter"></i>
        <i class="fab fa-youtube"></i>
        <i class="fab fa-instagram"></i>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
    name: 'CopyrightSection',
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

footer {
    height: 80px;
    background-color: black;

    .row {
      height: 100%;
    }

    .left-content,
    .right-content {
      height: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .left-content {
      color: $doveGrey;
      text-transform: uppercase;
      font-size: .8rem;

      span {
        color: $primaryWhite;
      }
    }

    .right-content {
      i {
        font-size: 1.2rem;
        color: white;
        padding: 0 10px;
      }
    }
}


</style>