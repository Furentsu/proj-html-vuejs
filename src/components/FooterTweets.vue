<template>
  <div class="col-3">
      <h3>Latest Tweets</h3>

      <div class="tweet">
          <div class="icon">
              <img src="../assets/images/3a74ce3d0532b7773b174c45ca3bd05a_bigger.png" alt="Tweet user image">
          </div>

          <div class="content-right">
              <h5>Theme Fusion</h5>
              <span>@Theme_Fusion</span>
              <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Molestias voluptatum fugit tenetur, at debitis ab ad unde facere odio odit officiis laborum aperiam illo nulla nostrum est ratione ut quo.</p>
              <div class="img-container">
                <img src="../assets/images/En2TRxLW4AEiWUN.jpeg" alt="WP Engine 30% off sale">
              </div>

              <div class="low-icons">
                  <div class="low-icons-left">
                      <i class="far fa-heart"></i>
                      <i class="fas fa-sign-out-alt"></i>
                  </div>

                  <div class="low-icons-right">
                      <span>22h</span>
                  </div>
              </div>
          </div>
      </div>
  </div>

</template>

<script>
export default {
    name: 'FooterTweets',
}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";


h3 {
    color: $vibrantBrightSun;
    font-size: 1.2rem;
    padding-bottom: 20px;
}

.tweet {
    
    display: flex;
    width: 100%;

    .icon {
        width: 20%;
        height: 100%;
        text-align: center;

        img {
            width: 35px;
            border-radius: 2em;
        }
    }

    .content-right {
        width: 80%;

        h5,
        p {
            color: $primaryWhite;
        }

        span {
            color: $doveGrey;
        }
        
        .img-container {
            width: 100%;

            img {
                width: 100%;
            }
        }

        .low-icons {
            display: flex;
            justify-content: space-between;

            .low-icons-left {
                color: $doveGrey;

                i {
                    padding: 10px 25px 0 0;
                }
            }

            .low-icons-right {
                padding-top: 8px;
            }
        }
    }
}

</style>