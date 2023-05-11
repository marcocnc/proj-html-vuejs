<script>
import { products } from '../../data/database'
export default {
    name: 'Products',
    data(){
        return{
            products
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
                <h5>titolo</h5>
                <h3 class="pb-3">Titolo</h3>

                <button class="btn btn-primary mt-5">Bottone</button>
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
        }
        .line{
            border-bottom: 1px solid white;
            margin: 150px 0;
        }
    }
</style>