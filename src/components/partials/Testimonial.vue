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
            <h5>OUR RECENT NEWS</h5>
            <h2 class="pb-3">OUR MOST POPULAR TESTIMONIAL POSTS</h2>
        </div> 

        <div class="mc-container">
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

                <!-- MADLEY PONDOR 1 -->
                <swiper-slide class="p-4">
                    <div class="slider-top d-flex justify-content-between w-100 align-items-center">
                        <div class="top-content d-flex">

                            <!-- IMAGE -->
                            <div class="top-image pe-2">
                                <img class="rounded-circle" src="../../../public/img/01 (2).jpg">
                            </div>
                            <div class="user text-start">
                                <h6 class="fs-5">MADLEY PONDOR</h6>
                                <span class="pt-2 text-start">UI Designer</span>
                            </div>
                        </div>

                        <!-- PARTNER IMAGE -->
                        <div class="user-partner">
                            <img class="animated" src="../../../public/img/01 (3).png">
                        </div>
                    </div>

                    <div class="line w-100 mt-4"></div>

                    <!-- REVIEW -->
                    <div class="review text-start pt-3">
                        <p class="fs-6">Edgeing nterfaces fnergstca plagiarize teams anbudng paradgms rapidiousl buildcaboration anden deassharing viaing and bleeding whereas goingi forward process and monetze</p>
                        <div class="rate d-flex pt-1 align-items-center">
                            <div class="stars me-2">
                                <i class="fa-regular fa-star mx-1" v-for="star in 5" :key="star" style="background-color: #00B67A;"></i>
                            </div>
                            <div class="number">
                                <span class="green-span">5.28</span>
                            </div>
                        </div>
                    </div>
                </swiper-slide>


                <!-- OLIVER BEDDOWS 1 -->
                <swiper-slide class="p-4">
                    <div class="slider-top d-flex justify-content-between w-100 align-items-center">
                        <div class="top-content d-flex">
                            <!-- IMAGE -->
                            <div class="top-image pe-2">
                                <img class="rounded-circle" src="../../../public/img/02 (3).jpg">
                            </div>
                            <div class="user text-start">
                                <h6 class="fs-5">OLIVER BEDDOWS</h6>
                                <span class="pt-2 text-start">UI Designer</span>
                            </div>
                        </div>
                        <!-- PARTNER IMAGE -->
                        <div class="user-partner">
                            <img class="animated" src="../../../public/img/01 (3).png">
                        </div>
                    </div>

                    <div class="line w-100 mt-4"></div>

                    <!-- REVIEW -->
                    <div class="review text-start pt-3">
                        <p class="fs-6">Rapidious buildcaboration anden deas sharing viaing and beedng edgeing nterfaces fnergstcia plagiarize teams anbuding paradgm whereas goingi forward process and monetze</p>
                        <div class="rate d-flex pt-1 align-items-center">
                            <div class="stars me-2">
                                <i class="fa-regular fa-star mx-1 rounded-circle" v-for="star in 5" :key="star" style="background-color: #F06A22;"></i>
                            </div>
                            <div class="number">
                                <span class="orange-span">5.28</span>
                            </div>
                        </div>
                    </div>
                </swiper-slide>


                <!-- MADLEY PONDOR 2 -->
                <swiper-slide class="p-4">
                    <div class="slider-top d-flex justify-content-between w-100 align-items-center">
                        <div class="top-content d-flex">

                            <!-- IMAGE -->
                            <div class="top-image pe-2">
                                <img class="rounded-circle" src="../../../public/img/01 (2).jpg">
                            </div>
                            <div class="user text-start">
                                <h6 class="fs-5">MADLEY PONDOR</h6>
                                <span class="pt-2 text-start">UI Designer</span>
                            </div>
                        </div>

                        <!-- PARTNER IMAGE -->
                        <div class="user-partner">
                            <img class="animated" src="../../../public/img/01 (3).png">
                        </div>
                    </div>

                    <div class="line w-100 mt-4"></div>

                    <!-- REVIEW -->
                    <div class="review text-start pt-3">
                        <p class="fs-6">Edgeing nterfaces fnergstca plagiarize teams anbudng paradgms rapidiousl buildcaboration anden deassharing viaing and bleeding whereas goingi forward process and monetze</p>
                        <div class="rate d-flex pt-1 align-items-center">
                            <div class="stars me-2">
                                <i class="fa-regular fa-star mx-1" v-for="star in 5" :key="star" style="background-color: #00B67A;"></i>
                            </div>
                            <div class="number">
                                <span class="green-span">5.28</span>
                            </div>
                        </div>
                    </div>
                </swiper-slide>



                <!-- OLIVER BEDDOWS 2 -->
                <swiper-slide class="p-4">
                    <div class="slider-top d-flex justify-content-between w-100 align-items-center">
                        <div class="top-content d-flex">
                            <!-- IMAGE -->
                            <div class="top-image pe-2">
                                <img class="rounded-circle" src="../../../public/img/02 (3).jpg">
                            </div>
                            <div class="user text-start">
                                <h6 class="fs-5">OLIVER BEDDOWS</h6>
                                <span class="pt-2 text-start">UI Designer</span>
                            </div>
                        </div>
                        <!-- PARTNER IMAGE -->
                        <div class="user-partner">
                            <img class="animated" src="../../../public/img/01 (3).png">
                        </div>
                    </div>

                    <div class="line w-100 mt-4"></div>

                    <!-- REVIEW -->
                    <div class="review text-start pt-3">
                        <p class="fs-6">Rapidious buildcaboration anden deas sharing viaing and beedng edgeing nterfaces fnergstcia plagiarize teams anbuding paradgm whereas goingi forward process and monetze</p>
                        <div class="rate d-flex pt-1 align-items-center">
                            <div class="stars me-2">
                                <i class="fa-regular fa-star mx-1 rounded-circle" v-for="star in 5" :key="star" style="background-color: #F06A22;"></i>
                            </div>
                            <div class="number">
                                <span class="orange-span">5.28</span>
                            </div>
                        </div>
                    </div>
                </swiper-slide>
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
        background-color: $color_darkblue;
    }

    .swiper-slide img {
        display: block;
        width: 100%;
        height: 100%;
        object-fit: cover;
    }
    // End Swiper Classes
    }

    .line{
        border-bottom: 1px solid #373E6C;
    }

    .stars i{
        padding: 8px;
    }

    .number .green-span{
        font-weight: 700;
        color: #00B67A;
    }

    .orange-span{
        color: #F06A22;
        font-weight: 700;
    }
</style>