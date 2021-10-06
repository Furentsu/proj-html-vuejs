<template>
   <main>

      <!-- Section between the jumbotron and the construction services offered  -->
      <section class="construction-projects-top">
          <h2>Do You Have A Construction Project We Can Help With?</h2>
          <button>Get a free quote</button>
      </section>

      <!-- Section containing the construction services  -->
      <section class="construction-projects-bottom">
          
      </section>

   </main>
</template>

<script>
export default {
  name: 'Main',
}
</script>


<style lang="scss" scoped>
@import "../style/variables.scss";

.construction-projects-top {
border: 1px solid red;

    display: flex;
    position: relative;
    justify-content: center;
    align-items: center;
    height: 130px;

    button {
        position: absolute;
        bottom: -15px;
    }

}

</style>