<template>
    <div class="final-jumbo pt-5 pb-5">

      <!-- Left content of the jumbotron -->
       <div class="left-content float-start">
           <div class="content">
                <h2 class="fw-light">Building inspiring spaces</h2>
                <div class="line"></div>
                <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Autem repellat, saepe maxime doloribus in voluptatem amet consequuntur beatae aspernatur ut possimus nobis rem, qui at assumenda fuga, quos totam iste!</p>
           </div>
       </div>

       <!-- Right content of the jumbotron -->
       <div class="right-content float-start">
            <button>Get a free quote</button>
            <p>Only takes a few seconds!</p>
       </div>
   </div>
</template>

<script>
export default {
  name: 'FinalJumbotron',
}
</script>


<style lang="scss" scoped>
@import "../style/variables.scss";

.final-jumbo {
    display: flex;
    justify-content: center;
    
    background-image: url('../assets/images/about-call-to-action-57862405.jpg');
    background-size: cover;
    background-position: bottom;


    .left-content,
    .right-content {
        width: 40%;
        height: 100%;
        padding: 50px 0;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;

        h2 {
            color: $primaryWhite;
        }

        p {
           color: $primaryWhite;
        }
    }

    .left-content {
        .content {
            text-align: left;

            .line {
                height: 2px;
                width: 30%;
                margin: 25px 0;
                background-color: $vibrantBrightSun;
             }
        }
    }

    .right-content {
        button {
            margin: 20px 10px;
            border: none;
            padding: 10px 50px;
            background-color: $vibrantBrightSun;
            color: $doveGrey;
            text-transform: uppercase;

            &:hover {
                    background-color: $codGrey;
                    color: $primaryWhite;
                }
        }
    }

}

</style>