
<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
export default {
    name:'Jumbotron',
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      return {};
    },
}
</script>

<template>
  
    <section id="jumbotron">

        <swiper class="mySwiper"
        :loop="true"
        >
            <!-- First slide -->
            <swiper-slide class="first-slide">
              <div class="mc-container h-100 text-white d-flex align-items-center">
                <div class="text text-start">
                  <h1>ONLINE GAME</h1>
                  <h2>GENUINE MONEY TRANSACTION</h2>

                  <p class="w-50 text-start">Assertively communicate an expanded array of mindshare rather than diverse technologies for magnetic applications eamlessly virtual then Conveniently monetize synergistic human capital</p>

                  <button class="mc-buttons jumbo-btn text-white">
                    <span>JOIN US TODAY</span>
                    <i class="fa-solid fa-circle-play ps-2"></i>
                  </button>
                </div>
              </div>
            </swiper-slide>
            
            
            <!-- Second slide -->
            <swiper-slide class="second-slide">
              <div class="mc-container h-100 text-white d-flex align-items-center">
                <div class="text text-start">
                  <h1>ONLINE GAME</h1>
                  <h2>GENUINE MONEY TRANSACTION</h2>

                  <p class="w-50 text-start">Assertively communicate an expanded array of mindshare rather than diverse technologies for magnetic applications eamlessly virtual then Conveniently monetize synergistic human capital</p>

                  <button class="jumbo-btn text-white">
                    <span>JOIN US TODAY</span>
                    <i class="fa-solid fa-circle-play ps-2"></i>
                  </button>
                </div>
              </div>
            </swiper-slide>
          </swiper>
    </section>
</template>

<style lang="scss" scoped>
@use '../../scss/partials/vars' as *;
    #jumbotron{
    .swiper {
        width: 100%;
        height: 100%;
      }

      .swiper-slide {
        text-align: center;
        font-size: 18px;
        background: #fff;
        display: flex;
        justify-content: center;
        align-items: center;
      }

      .swiper-slide img {
        display: block;
        width: 100%;
        height: 100%;
        object-fit: cover;
      }

      .first-slide,
      .second-slide{
          height: 700px;
          .text{
            h1{
              font-size: 90px;
              font-weight: 700;
              text-shadow: 2px 2px darken($color_red, $amount: 10%);
            }

            p{
              line-height: 30px;
              font-size: 15px;
            }
          }

          .jumbo-btn{
            box-shadow: 4px 4px #D0D4D8;
            background-color: $color_white;

            &:hover{
              background-color: $color_red;
              box-shadow: -4px -4px $color_white;
              transition: all .3s;
            }

            &:hover span, &:hover i{
              color: $color_white;
            }

            span, i{
              color: $color_red;
            }
          }
      }

      .first-slide{
          background-image: url('../../../public/img/bg.jpg');
          background-position: center;

          
      }

      .second-slide{
          background-image: url('../../../public/img/bg-2.jpg');
          background-position: center;
      }
    }
</style>