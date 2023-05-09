<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import { Autoplay, Navigation } from 'swiper';
export default {
    name: 'Squads',
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
    <section class="squads">
        <div class="titles text-center pt-5">
            <h5>titolo</h5>
            <h3>Titolo</h3>
        </div> 

        <swiper
            :slidesPerView="5"
            :spaceBetween="25"
            :centeredSlides="true"
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
            <swiper-slide>Slide 1</swiper-slide>
            <swiper-slide>Slide 2</swiper-slide><swiper-slide>Slide 3</swiper-slide>
            <swiper-slide>Slide 4</swiper-slide><swiper-slide>Slide 5</swiper-slide>
            <swiper-slide>Slide 6</swiper-slide><swiper-slide>Slide 7</swiper-slide>
            <swiper-slide>Slide 8</swiper-slide><swiper-slide>Slide 9</swiper-slide>
        </swiper>
    </section>
</template>

<style lang="scss" scoped>
  .squads{
    background-color: red;
    padding-bottom: 120px;

    // Swiper classes
    .swiper {
        width: 100%;
        height: 100%;
    }

    .swiper-slide {
        height: 400px;
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