
<script>
import {upcomingMatch, previousMatch} from '../../data/database';
export default {
    name: 'Schedule',
    data(){
        return{
            upcomingMatch,
            previousMatch
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
    <section class="schedule pt-5">
        <div class="mc-container d-flex flex-column justify-content-center align-items-center">
            <h5>ANYWHERE, ANYTIME</h5>
            <h2>ALL MATCHES SCHEDULE</h2>

            <!-- Main Match -->
            <div class="main-match w-100 my-4">

                <!-- Top with red band -->
                <div class="red-band px-4 py-2 d-flex justify-content-between">

                    <div class="left-side">
                        <span class="pe-2 fs-5">2 GROUP</span>
                        <span class="fs-5 bold-span">32 PLAYERS</span>
                    </div>
                    <div class="right-side">
                        <span class="pe-2 fs-5">PRIZE POOL</span>
                        <span class="fs-5 bold-span">$3200</span>
                    </div>
                </div>

                <!-- White band with match informations -->
                <div class="white-band p-4">
                    <div class="row align-items-center">

                        <!-- Tournament -->
                        <div class="col-4">
                            <h4 class="text-black">BATTLEFIELD-4 TOURNAMENT</h4>
                            <div class="match-data d-flex justify-content-between">
                                <span class="day pe-2">30 April 2022</span>
                                <span>Time: 08:30PM</span>
                            </div>
                        </div>

                        <!-- Teams images -->
                        <div class="col-4 d-flex justify-content-between align-items-center">
                            <a href="#">
                                <img src="../../../public/img/teamsm-6.png" alt="teamsm-6">
                            </a>
                            <a href="#">
                                <img class="vs-image" src="../../../public/img/vs.png" alt="vs">
                            </a>
                            <a href="#">
                                <img src="../../../public/img/teamsm-9.png" alt="teamsm-9">
                            </a>
                       </div>

                        <!-- Socials and button -->
                        <div class="col-4 d-flex align-items-center">
                            <div class="social pe-2">
                                <a href="#" class="pe-2">
                                     <img src="../../../public/img/social-1.png" alt="social-1">
                                </a>

                                <a href="#" class="pe-2">
                                    <img src="../../../public/img/social-2.png" alt="social-2">
                                </a>

                                <a href="#">
                                    <img src="../../../public/img/social-3.png" alt="social-3">
                                </a>
                            </div>

                            <div class="match-button">
                                <button class="mc-buttons-reverse">WATCH NOW <i class="fa-solid fa-circle-play"></i></button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <!-- All Matches -->
            <div class="all-matches d-flex w-100">

                <!-- Upcoming -->
                <div class="upcoming d-flex flex-column w-50 me-4">
                    <h4 class="text-center">UPCOMING MATCHES</h4>

                    <div class="match w-100 h-100 my-4" v-for="(match, index) in upcomingMatch" :key="index">

                        <div class="red-band px-4 py-2 d-flex justify-content-between">

                            <div class="left-side">
                                <span class="pe-2 fs-5">2 GROUP</span>
                                <span class="fs-5 bold-span">32 PLAYERS</span>
                            </div>
                            <div class="right-side">
                                <span class="pe-2 fs-5">PRIZE POOL</span>
                                <span class="fs-5 bold-span">$3200</span>
                            </div>
                        </div>

                        <!-- White band with match informations -->
                        <div class="white-band p-4">
                            <div class="row align-items-center">

                                <!-- FIRST TEAM IMAGE -->
                                <div class="col-4 w-25 d-flex align-items-center justify-content-center">
                                    <a href="#">
                                        <img :src="getImage(`../../../public/img/${match.firstTeam}.png`)">
                                    </a>
                                </div>

                                <!-- MATCH INFO -->
                                <div class="col-4 w-50">
                                    <h4 class="text-black fs-5">{{ match.nameTournament }}</h4>
                                    <div class="text-grey d-flex justify-content-center">
                                        <span class="day pe-2">30 April 2022</span>
                                        <span>Time: 08:30PM</span>
                                    </div>
                                    <div class="social d-flex justify-content-center pe-2 pt-3">
                                        <a href="#" class="pe-2">
                                            <img src="../../../public/img/social-1.png" alt="social-1">
                                        </a>

                                        <a href="#" class="pe-2">
                                            <img src="../../../public/img/social-2.png" alt="social-2">
                                        </a>

                                        <a href="#">
                                            <img src="../../../public/img/social-3.png" alt="social-3">
                                        </a>
                                    </div>
                                </div>

                                <!-- SECOND TEAM IMAGE -->
                                <div class="col-4 d-flex align-items-center justify-content-center w-25">
                                    <a href="#">
                                        <img :src="getImage(`../../../public/img/${match.secondTeam}.png`)">
                                    </a>
                                </div>
                            </div>
                        </div>
                    </div>

                </div>            

                <!-- Previous -->
                <div class="previous d-flex flex-column w-50">
                    <h4 class="text-center">PREVIOUS MATCHES</h4>
                     <div class="match w-100 my-4 h-100" v-for="(match, index) in previousMatch" :key="index">

                        <div class="red-band px-4 py-2 d-flex justify-content-between">

                            <div class="left-side">
                                <span class="pe-2 fs-5">2 GROUP</span>
                                <span class="fs-5 bold-span">32 PLAYERS</span>
                            </div>
                            <div class="right-side">
                                <span class="pe-2 fs-5">PRIZE POOL</span>
                                <span class="fs-5 bold-span">$3200</span>
                            </div>
                        </div>

                        <!-- White band with match informations -->
                        <div class="white-band p-4">
                            <div class="row align-items-center">

                                <!-- FIRST TEAM IMAGE -->
                                <div class="col-4 w-25 d-flex align-items-center justify-content-center">
                                    <a href="#">
                                        <img class="match-team-image" :src="getImage(`../../../public/img/${match.firstTeam}.png`)">
                                    </a>
                                </div>

                                <!-- MATCH INFO -->
                                <div class="col-4 w-50">
                                    <h4 class="text-black text-center fs-5">{{ match.nameTournament }}</h4>
                                    <div class="text-grey d-flex justify-content-center">
                                        <span class="day pe-2">30 April 2022</span>
                                        <span>Time: 08:30PM</span>
                                    </div>
                                    <div class="social d-flex justify-content-center pe-2 pt-3">
                                        <a href="#" class="pe-2">
                                            <img src="../../../public/img/social-1.png" alt="social-1">
                                        </a>

                                        <a href="#" class="pe-2">
                                            <img src="../../../public/img/social-2.png" alt="social-2">
                                        </a>

                                        <a href="#">
                                            <img src="../../../public/img/social-3.png" alt="social-3">
                                        </a>
                                    </div>
                                </div>

                                <!-- SECOND TEAM IMAGE -->
                                <div class="col-4 d-flex align-items-center justify-content-center w-25">
                                    <a href="#">
                                        <img class="match-team-image" :src="getImage(`../../../public/img/${match.secondTeam}.png`)">
                                    </a>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div class="mc-buttons my-5">BROWSE ALL MATCHES <i class="fa-solid fa-chevron-right fs-6"></i></div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
@use '../../scss/partials/vars' as *;

    .schedule{
        background-image: url('../../../public/img/bg\ \(1\).jpg');
        background-size: cover;
        background-position: center;
        padding-bottom: 120px;

        h4{
            font-weight: 700;
        }

        .main-match, .match{
            .red-band{
                background-color: $color_red;
                .bold-span{
                    font-weight: 700;
                }
            }

            .white-band{
                background-color: $color_white;
                
            }
            .match-data{
                color: #555;
                width: 55%;
                .day{
                    border-right: 2px solid #555;
                }
            }
        }

        .upcoming, .previous{
            .text-grey{
                color: #555;
            }
        }

        .previous{
            .match-team-image{
                width: 85px;
                height: 85px;
            }
        }
    }
</style>