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
            <h3 class="pb-3">Titolo</h3>
        </div> 

        <!-- Swiper -->
        <swiper
            :slidesPerView="5"
            :spaceBetween="20"
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
            <swiper-slide>Slide 10</swiper-slide>
        </swiper>
        <!-- End Swiper -->

        <div class="mc-container ">
            <div class="community d-flex w-100">
                <div class="community-txt p-5 w-50">
                    <span>titolo</span>
                    <h3>Titolo</h3>
                    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Unde iure, nesciunt blanditiis distinctio recusandae aliquid quo mollitia in perspiciatis tempora dolor cumque nulla? Quaerat, quae ullam! Voluptatem vel veritatis perferendis!</p>
                    <button class="btn btn-primary">bottone</button>
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
}


</style>