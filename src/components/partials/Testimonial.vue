<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Autoplay, Navigation } from 'swiper';
export default {
    name: 'Testimonial',
    components: {
      Swiper,
      SwiperSlide,
    },
    setup() {
      return {
        modules: [Autoplay, Navigation]
      }
    }
}
</script>

<template>
    <section class="testimonial">
        <div class="titles text-center pt-5">
            <h5>titolo</h5>
            <h3 class="pb-3">Titolo</h3>
        </div> 

        <div class="mc-container text-black">
            <swiper
                :slidesPerView="2"
                :spaceBetween="10"
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
                <swiper-slide>Slide 1</swiper-slide><swiper-slide>Slide 2</swiper-slide>
                <swiper-slide>Slide 3</swiper-slide><swiper-slide>Slide 4</swiper-slide>
            </swiper>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../scss/partials/vars' as *;

    .testimonial{
        background-image: url('../../../public/img/bg.png');
        background-size: contain;
        padding-bottom: 130px;
        background-color: darken($color_blue, $amount: 10%);
        
        .mySwiper{
            margin-bottom: 110px;
        }
        .swiper {
            width: 100%;
            height: 100%;
        }

    .swiper-slide {
        height: 300px;
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
    // End Swiper Classes
    }
</style>