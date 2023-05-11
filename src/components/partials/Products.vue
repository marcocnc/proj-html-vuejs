<script>
import { products, partnersList1, partnersList2 } from '../../data/database'
export default {
    name: 'Products',
    data(){
        return{
            products,
            partnersList1,
            partnersList2
        }
    },
    methods:{
        getImage(img){
            return new URL(img, import.meta.url).href;
        }
    }
}
</script>

<template>
    <section class="products pt-5">
        <div class="mc-container">
            <div class="titles text-center pt-5">
                <h5>GAMER T-SHIRT’S</h5>
                <h2 class="pb-3">EXPLORE OUR PRODUCTS</h2>
            </div> 
                <!-- Row with 4 col -->
                <div class="row">
                    <div class="col-3" 
                    v-for="(product, index) in products" 
                    :key="index">

                        <!-- Product DIV -->
                        <div class="product p-3">     

                            <!-- Product image -->
                            <div class="product-image">
                                <img class="w-100" :src="getImage(`../../../public/img/${product.img} (1).jpg`)">
                            </div>

                            <!-- Product text -->
                            <div class="product-text text-center pt-4">
                                <h4 class="fs-5"> {{ product.color }} T-SHIRT HERE</h4>
                                <h6 class="fs-5">$380.00</h6>
                                <div class="stars d-flex justify-content-center pt-2">
                                    <i class="fa-solid fa-star" v-for="star in 5" :key="star"></i>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
              

            <div class="line w-100"></div>

            <div class="titles text-center pt-5">
                <h5>WE OUR PARTNERS</h5>
                <h2 class="pb-3">BECOME A PARTNER OF GAMER</h2>

                <div class="row pt-3">
                    <div class="first-col d-flex justify-content-center">
                        <div class="partner" 
                        v-for="(partner, index) in partnersList1"
                        :key="index"
                        >
                            <img class="me-5" :src="getImage(`../../../public/img/${partner.img}.png`)">
                        </div>
                    </div>

                    <div class="second-col d-flex justify-content-center pt-5">
                        <div class="partner"
                        v-for="(partner, index) in partnersList2"
                        :key="index">
                        <img class="me-5" :src="getImage(`../../../public/img/${partner.img}.png`)">
                        </div>
                    </div>
                </div>
                <button class="mc-buttons my-5">BECOME A PARTNER <i class="fa-solid fa-circle-chevron-right"></i></button>
            </div>
        </div>
    </section>                
</template>

<style lang="scss" scoped>
@use '../../scss/partials/vars' as *;
    .products{
        background-color: darken($color_blue, $amount: 10%);
        padding-bottom: 120px;

        .product{
            background-color: $color_darkblue;
            cursor: pointer;

            &:hover{
                background-color: $color_red;
                transition: all .5s;
            }
        }

        .product-image{
            overflow: hidden;
            img{
                &:hover{
                    transform:rotate(15deg) scale(1.2);
                    transition: all .3s;
                }
            }
        }
        .line{
            border-bottom: 1px solid white;
            margin: 150px 0;
        }
    }
</style>