<script>
export default {
    name: 'RecentNews'
}
</script>

<template>
    <section class="recent-news">

        <div class="titles text-center pt-5">
            <h5>OUR RECENT NEWS</h5>
            <h2 class="pb-3">OUR MOST POPULAR BLOG POSTS</h2>
        </div> 
            <div class="mc-container">
                <div class="row">

                    <!-- First col -->
                    <div class="col-6 p-3">
                        <div class="news">
                            <div class="news-image">
                                <img src="../../../public/img/01 (3).jpg" alt="">
                            </div>

                            <div class="news-content p-3 text-start">
                                <h4>DISTINCTIVE REDEFINE RESOURCE MAXIMIZING FOR</h4>

                                <div class="type-data">
                                    <span class="pe-2">Admin</span>
                                    <span class="ps-2">01 January 2022</span>
                                </div>

                                <p class="pt-3">Uniquely conceptuaze visionary process ariwith tactical ramatica centered qualitys vectoris with outofthebox scenario is ompelling uthoritatively generate front-end niches after one</p>

                                <button class="mc-buttons-reverse mt-3">READ MORE</button>
                            </div>
                        </div>
                    </div>

                    <!-- Second col -->
                    <div class="col-6 p-3">
                        <div class="news">
                            <div class="news-image">
                                <img src="../../../public/img/02 (2).jpg" alt="">
                            </div>

                            <div class="news-content p-3 text-start">
                                <h4>REDEFINE RESOURCE MAXIMIZING FOR DISTINCTIVE</h4>

                                <div class="type-data">
                                    <span class="pe-2">Admin</span>
                                    <span class="ps-2">01 January 2022</span>
                                </div>

                                <p class="pt-3">Uniquely conceptuaze visionary process ariwith tactical ramatica centered qualitys vectoris with outofthebox scenario is ompelling uthoritatively generate front-end niches after one</p>

                                <button class="mc-buttons-reverse mt-3">READ MORE</button>
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
        
        .news{
            background-color: $color_darkblue;
            .news-image{
                border: 10px solid $color_darkblue;
                img{
                    width: 100%;
                    object-fit: cover;
                }
            }
        }

        .type-data span:first-child{
            border-right: 1px solid white;
        }
    }

</style>