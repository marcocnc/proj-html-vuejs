<script>
export default {
    name: 'Products'
}
</script>

<template>
    <section class="products pt-5">
        <div class="mc-container">
            <div class="titles text-center pt-5">
                <h5>titolo</h5>
                <h3 class="pb-3">Titolo</h3>

                <!-- Row with 4 col -->
                <div class="row">
                    <div class="col-3">
                        <div class="product p-3 border">     

                            <!-- Product image -->
                            <div class="product-image">
                                <img src="../../../public/img/01 (1).jpg" alt="">
                            </div>

                            <!-- Product text -->
                            <div class="product-text pt-4">
                                <h3>titolo</h3>
                                <h3>costo</h3>
                                <h3>stelle</h3>
                            </div>
                        </div>
                    </div>

                    <div class="col-3">
                        <div class="product p-3 border">     

                            <!-- Product image -->
                            <div class="product-image">
                                <img src="../../../public/img/01 (1).jpg" alt="">
                            </div>

                            <!-- Product text -->
                            <div class="product-text pt-4">
                                <h3>titolo</h3>
                                <h3>costo</h3>
                                <h3>stelle</h3>
                            </div>
                        </div>
                    </div>

                    <div class="col-3">
                        <div class="product p-3 border">     

                            <!-- Product image -->
                            <div class="product-image">
                                <img src="../../../public/img/01 (1).jpg" alt="">
                            </div>

                            <!-- Product text -->
                            <div class="product-text pt-4">
                                <h3>titolo</h3>
                                <h3>costo</h3>
                                <h3>stelle</h3>
                            </div>
                        </div>
                    </div>

                    <div class="col-3">
                        <div class="product p-3 border">     

                            <!-- Product image -->
                            <div class="product-image">
                                <img src="../../../public/img/01 (1).jpg" alt="">
                            </div>

                            <!-- Product text -->
                            <div class="product-text pt-4">
                                <h3>titolo</h3>
                                <h3>costo</h3>
                                <h3>stelle</h3>
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

        .line{
            border-bottom: 1px solid white;
            margin: 150px 0;
        }
    }
</style>