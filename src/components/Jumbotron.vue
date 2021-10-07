<template>
    <div class="jumbo">

      <!-- Central content of the jumbotron -->
       <div class="jumbo-content">
            <h1 class="fw-bold text-white">Building inspiring spaces</h1>
            <h2 class="fs-5">We Build Inspiring Residential &#38; Commercial Spaces</h2>
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

        h1 {
            font-size: 3.5rem;
        }

        h2 {
            color: $vibrantBrightSun;
        }

        button {
            margin: 20px 10px;
            border: none;
            padding: 10px 50px;

            &:nth-of-type(1) {
                background-color: $codGrey;
                color: $primaryWhite;
            }

            &:nth-of-type(2) {
                background-color: $brightSun;
            }
        }


    }

    .jumbo-squares {
        position: absolute;
        top: 10px;
        right: 15px;
        text-align: center;

        .demos,
        .sales {
            margin: 10px 0;
            width: 70px;
            height: 70px;
            color: $primaryWhite;
        }
    }

}

</style>