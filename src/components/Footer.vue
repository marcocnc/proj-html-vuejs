
<script>
import { footerTopInfo, topJackpotGames } from '../data/database';
export default {
    name:'Footer',
    data(){
        return{
            footerTopInfo,
            topJackpotGames
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
    <footer>
        <div class="footer-top">

            <div class="mc-container">

                <!-- Row with phone, mail and address -->
                <div class="row">

                    <div class="col-4 p-4 infos d-flex align-items-center" 
                    v-for="(info, index) in footerTopInfo"
                    :key="index"
                    >
                        <div class="image me-3">
                            <img :src="getImage(`../../public/img/${info.img} (4).png`)">
                        </div>
                        <div class="text">
                            <span>{{ info.text }}</span>
                        </div>
                    </div>

                </div>
            </div>
        </div>

        <!-- Footer center -->
        <div class="footer-center">
            <div class="mc-container">
                <div class="row">

                    <!-- Logo and Brands div -->
                    <div class="col-4 logo-brands">
                        <div class="logo">
                            <img src="../../public/img/logo.png" alt="logo">
                        </div>
                        <p class="pt-3">Upropriate brand economca sound technolog after covalent technology enable prospective wastng markets whereas propriate and brand economca sound technolog</p>
                        <div class="brands d-flex">
                            <img class="me-2" src="../../public/img/social-1.png">
                            <img class="me-2" src="../../public/img/social-2.png">
                            <img src="../../public/img/social-3.png">
                        </div>
                    </div>

                    <!-- Teams div -->
                    <div class="col-4 jackpot">
                        <h4>TOP JACKPOT GAMES</h4>
                        <div class="teams pt-3">

                            <!-- Teams -->
                            <div class="team d-flex pt-2" 
                            v-for="(team, index) in topJackpotGames"
                            :key="index">
                                <div class="team-img">
                                    <img :src="getImage(`../../public/img/${team.img} (5).jpg`)">
                                </div>
                                <div class="team-content ps-3">
                                    <h6>{{team.title}} POKER GAME</h6>
                                    <span class="poker">Poker: <span class="dollars"> {{team.poker}}</span> </span>
                                    <div class="stars">
                                        <i class="fa-solid fa-star me-1 pt-2" v-for="star in 5" :key="star"></i>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Newsletter -->
                    <div class="col-4 newsletter">
                        <h4>OUR NEWSLETTER</h4>
                        <p class="pt-3">Gamer esports organization supported by community leaders</p>

                        <input type="text" placeholder="Your name" class="p-3 w-100">
                        <input type="text" placeholder="Your email" class=" mt-4 p-3 w-100">

                        <button class="mc-buttons my-5">SEND MESSAGE <i class="fa-solid fa-circle-chevron-right"></i></button>
                    </div>
                </div>
            </div>
        </div>
        <!-- End Footer center -->
    </footer>
    <!-- Footer bottom -->
    <div class="footer-bottom d-flex justify-content-center align-items-center">
        <span> ©2023 Marco Cancelliere - Boolean #94 &hearts; </span>
    </div>
</template>

<style lang="scss" scoped>
@use '../scss/partials/vars' as *;

    footer{
        background-image: url('../../public/img/bg\ \(3\).jpg');
        background-size: cover;
        padding-bottom: 150px;
        .footer-top{
            border-bottom: 1px solid #1E1E3E;
            margin-bottom: 80px;

            .infos{
                border-left: 1px solid #1E1E3E;

                &:last-child{
                    border-right: 1px solid #1E1E3E;
                }
            }
        }
        
    }

    .footer-center{

        .team-img{
            img{
                width: 80px;
                height: 80px;
            }
        }
        .poker, .dollars{
            font-size: 13px;
        }
        .dollars{
            font-weight: 700;
        }

        .stars{
            font-size: 14px;
            color: $color_red;
        }

        input{
            background-color: $color_darkblue;
            border: none;
            color: $color_white;

            &:focus{
                outline: none;
            }
        }
    }
    .footer-bottom{
        height: 90px;
        background-color: $color_darkblue;
    }
</style>