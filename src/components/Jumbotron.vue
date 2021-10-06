<template>
    <div class="jumbo">

      <!-- Central content of the jumbotron -->
       <div class="jumbo-content">
            <h1>Building inspiring spaces</h1>
            <h2>We Build Inspiring Residential &#38; Commercial Spaces</h2>
            <button>Explore recent work</button>  
            <button>Get a quote today</button>  
       </div>

       <!-- Top right squares with demos and sales -->
       <div class="jumbo-squares">
            <div class="demos">
               <span>Demos</span>
            </div>

            <div class="sales">
               <span>On sale</span>
            </div>
       </div>
   </div>
</template>

<script>
export default {
  name: 'Jumbotron',
}
</script>


<style lang="scss" scoped>
@import "../style/variables.scss";

.jumbo {
    height: 600px;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    background-image: url('../assets/images/home-slider-62528242.jpg');
    background-size: cover;

    .jumbo-content {
        width: fit-content;
        text-align: center;
    }

    .jumbo-squares {
        position: absolute;
        top: 10px;
        right: 10px;
        text-align: center;

        .demos,
        .sales {
            border: 1px solid white;
            margin: 10px 0;
            width: 70px;
            height: 70px;
        }
    }

}

</style>