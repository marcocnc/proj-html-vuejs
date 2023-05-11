<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Autoplay, Navigation } from 'swiper';
import {squadPlayers} from '../../data/database';

export default {
    name: 'Squads',
    components: {
      Swiper,
      SwiperSlide,
    },
    data(){
        return{
            squadPlayers
        }
    },
    methods:{
        getImage(img){
            return new URL(img, import.meta.url).href;
        }
    },

    setup() {
      return {
        modules: [Autoplay, Navigation]
      }
    }
    
}
</script>

<template>
    <section class="squads">
        <div class="titles text-center pt-5">
            <h5>OUR TEAM PLAYERS</h5>
            <h2 class="pb-3">MEET OUR SQUAD PLAYERS</h2>
        </div> 

        <!-- Swiper -->
        <swiper
            :slidesPerView="5"
            :spaceBetween="30"
            :centeredSlides="false"
            :autoplay="{
            delay: 2500,
            disableOnInteraction: false,
            }"
            :pagination="{
            clickable: true,
            }"
            :navigation="true"
            :modules="modules"
            :loop="true"
            class="mySwiper"
        >
            
            <!-- First group of slides -->
            <swiper-slide class="d-flex flex-column" v-for="(squad, index) in squadPlayers"
             :key="index" 
             :style="`background-image: url('../../../public/img/${index + 1}.jpg')`">

                <div class="image">
                    <img :src="getImage(`../../../public/img/${squad.img}.png`)">
                </div>

                <div class="name-squad pt-3">
                    <h3>{{ squad.team }}</h3>
                </div>

                <div class="social d-flex">
                    <a href="#" class="pe-2">
                        <img src="../../../public/img/social-1.png" alt="social-1">
                    </a>

                    <a href="#" class="pe-2">
                        <img src="../../../public/img/social-2.png" alt="social-2">
                    </a>

                    <a href="#">
                        <img src="../../../public/img/social-3.png" alt="social-3">
                    </a>
                </div>
                    
            </swiper-slide>

            <!-- Second group of slides -->
            <swiper-slide class="d-flex flex-column"
             v-for="(squad, index) in squadPlayers"
              :key="index"
              :style="`background-image: url('../../../public/img/${index + 1}.jpg')`">

                <div class="image">
                    <img :src="getImage(`../../../public/img/${squad.img}.png`)">
                </div>

                <div class="name-squad pt-3">
                    <h3>{{ squad.team }}</h3>
                </div>

                <div class="social d-flex">
                    <a href="#" class="pe-2">
                        <img src="../../../public/img/social-1.png" alt="social-1">
                    </a>

                    <a href="#" class="pe-2">
                        <img src="../../../public/img/social-2.png" alt="social-2">
                    </a>

                    <a href="#">
                        <img src="../../../public/img/social-3.png" alt="social-3">
                    </a>
                </div>
                    
            </swiper-slide>
        </swiper>
        <!-- End Swiper -->

        <div class="mc-container ">
            <div class="community d-flex w-100">
                <div class="community-txt p-5 w-50">
                    <h5>LET'S PLAY TOGETHER</h5>
                    <h3>JOIN GAMER ESPORTS TO BECOME NEXT PRO GAMER TODAY!</h3>
                    <p class="py-4">Distinctively provide acces mutfuncto users whereas transparent proceses somes ncentivize eficient functionalities rather than an extensible archtectur services and cross</p>
                    <button class="mc-buttons">JOIN COMMUNITY <i class="fa-solid fa-chevron-right fs-6"></i></button>
                </div>
                <div class="community-image w-50">
                    <img src="../../../public/img/01 (1).png" alt="01">
                </div>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../scss/partials/vars' as *;
  .squads{
    background-color: darken($color_blue, $amount: 10%);
    padding-bottom: 120px;

    // Swiper classes
    .mySwiper{
        margin-bottom: 110px;
    }
    .swiper {
        width: 100%;
        height: 100%;
    }

    .swiper-slide {
        height: 450px;
        text-align: center;
        font-size: 18px;
        background: #fff;
        display: flex;
        justify-content: center;
        align-items: center;
        border: 10px solid $color_darkblue;
    }

    .swiper-slide img {
        display: block;
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
    // End Swiper Classes

    .community{
        background-image: url('../../../public/img/bg\ \(4\).jpg');
        background-size: cover;
        background-position: center;
    }

    .social{
        a{
            img{
                height: 50px;
                width: 50px;
            }
        }
    }
}


</style>