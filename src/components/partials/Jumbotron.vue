
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

        <swiper class="mySwiper">

            <swiper-slide class="first-slide">Slide 1</swiper-slide>
            <swiper-slide class="second-slide">Slide 2</swiper-slide>

        </swiper>
        <!-- <div class="mc-container h-100 text-white d-flex justify-content-start align-items-center">
            <div class="text">
                <h1>TITOLO</h1>
                <h2>TITOLO</h2>
                <p>Desc</p>
                <button class="btn btn-primary text-white">button</button>
            </div>
        </div> -->
    </section>
</template>

<style lang="scss" scoped>
    // #jumbotron{
    //     height: 700px;
    //     background: #000000a1;
    //     background-image: url(../../../public/img/bg.jpg);
    //     background-position: center;

    //     h1{
    //         font-size: 100px;
    //     }
    // }
    .swiper {
  width: 100%;
  height: 100%;
}

.swiper-slide {
  text-align: center;
  font-size: 18px;
  background: #fff;

  /* Center slide text vertically */
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
}

.first-slide{
    background-image: url('../../../public/img/bg.jpg');
}

.second-slide{
    background-image: url('../../../public/img/bg-2.jpg');
}
</style>