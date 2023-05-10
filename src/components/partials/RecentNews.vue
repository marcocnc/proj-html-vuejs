<script>
export default {
    name: 'RecentNews'
}
</script>

<template>
    <section class="recent-news">

        <div class="titles text-center pt-5">
            <h5>titolo</h5>
            <h3 class="pb-3">Titolo</h3>

            <div class="mc-container">
                <div class="row">

                    <!-- First col -->
                    <div class="col-6 p-3" style="background-color: red;">
                        <div class="news-image">
                            <img src="../../../public/img/01 (3).jpg" alt="">
                        </div>

                        <div class="news-content p-3 text-start">
                            <h5>DISTINCTIVE REDEFINE RESOURCE MAXIMIZING FOR</h5>

                            <div class="type-data">
                                <span class="pe-2">Admin</span>
                                <span class="ps-2">01 January 2022</span>
                            </div>

                            <p class="pt-3">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Repudiandae, molestias quos delectus aspernatur quia veritatis temporibus ut dolores adipisci optio, vel nesciunt enim dolore tenetur error, molestiae voluptatum commodi praesentium!</p>

                            <button class="btn btn-primary mt-3">Button</button>
                        </div>
                    </div>

                    <!-- Second col -->
                    <div class="col-6 p-3" style="background-color: blue;">
                        <div class="news-image">
                            <img src="../../../public/img/01 (3).jpg" alt="">
                        </div>

                        <div class="news-content p-3 text-start">
                            <h5>DISTINCTIVE REDEFINE RESOURCE MAXIMIZING FOR</h5>

                            <div class="type-data">
                                <span class="pe-2">Admin</span>
                                <span class="ps-2">01 January 2022</span>
                            </div>

                            <p class="pt-3">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Repudiandae, molestias quos delectus aspernatur quia veritatis temporibus ut dolores adipisci optio, vel nesciunt enim dolore tenetur error, molestiae voluptatum commodi praesentium!</p>

                            <button class="btn btn-primary mt-3">Button</button>
                        </div>
                    </div>
                </div>
            </div>
        </div> 
    </section>
</template>

<style lang="scss" scoped>
@use '../../scss/partials/vars' as *;

    .recent-news{
        background-image: url('../../../public/img/bg\ \(2\).jpg');
        padding-bottom: 150px;
        .news-image{
            img{
                width: 100%;
                object-fit: cover;
            }
        }

        .type-data span:first-child{
            border-right: 1px solid white;
        }
    }

</style>