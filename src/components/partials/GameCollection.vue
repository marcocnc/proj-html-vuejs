<script>
export default {
    name:'GameCollection'
}
</script>

<template>
    
    <!-- Our Game Collections -->
    <section class="game-collections pt-5">

        <div class="mc-container">
            <div class="top d-flex flex-column justify-content-center align-items-center pt-5">
                <h5>TODAY'S</h5>
                <h2>OUR GAME COLLECTION</h2>

                <!-- Cards -->
                <div class="mc-cards-container w-100 d-flex mt-4">
                    <div class="mc-card d-flex justify-content-center align-items-center">
                        <img class="team-image" src="../../../public/img/team-1.png" alt="team-1">
                        <img class="vs-image mx-3" src="../../../public/img/vs.png" alt="vs">
                        <img class="team-image" src="../../../public/img/team-2.png" alt="team-2">
                    </div>

                    <div class="mc-card d-flex justify-content-center align-items-center">
                        <img class="team-image" src="../../../public/img/teamsm-4.png" alt="team-1">
                        <img class="vs-image mx-3" src="../../../public/img/vs.png" alt="vs">
                        <img class="team-image" src="../../../public/img/teamsm-3.png" alt="team-2">
                    </div>

                    <div class="mc-card d-flex justify-content-center align-items-center">
                        <img class="team-image" src="../../../public/img/teamsm-2.png" alt="team-1">
                        <img class="vs-image mx-3" src="../../../public/img/vs.png" alt="vs">
                        <img class="team-image" src="../../../public/img/teamsm-1.png" alt="team-2">
                    </div>
                </div>

                <div class="mc-buttons my-5">BROWSE ALL GAMES <i class="fa-solid fa-chevron-right fs-6"></i></div>
            </div>

            <div class="line w-100"></div>

            <!-- Who we are -->
            <div class="bottom d-flex justify-content-between pb-5">
                <div class="who-image w-50">
                    <img src="../../../public/img/01.png" alt="01">
                </div>
                <div class="who-text w-50 ps-3">
                    <div class="titles pt-5">
                        <h5>WHO WE ARE</h5>
                        <h2 class="pb-3 w-75">WE ARE PROFESSIONAL TEAM ESPORT</h2>
                        <p class="w-75">
                            Distinctively provide acces mutfuncto users whereas transparent proceses somes ncentivize eficient functionalities rather than an extensible archtectur services and cross
                        </p>

                        <!-- Info div -->
                        <div class="infos">
                            <div class="info d-flex">
                                <div class="info-image me-3">
                                    <img class="p-3" src="../../../public/img/icon-1.png" alt="icon-1">
                                </div>
                                <div class="info-text">
                                    <h5 class="text-white">103K COMMUNITY EARNING</h5>
                                    <p>Distinctively provide acces mutfuncto users whereas communicate leveraged services</p>
                                </div>
                            </div>

                            <div class="info d-flex">
                                <div class="info-image me-3">
                                    <img class="p-3" src="../../../public/img/icon-2.png" alt="icon-1">
                                </div>
                                <div class="info-text">
                                    <h5 class="text-white">34M+ REGISTERED PLAYERS</h5>
                                    <p>Distinctively provide acces mutfuncto users whereas communicate leveraged services</p>
                                </div>
                            </div>

                            <div class="info d-flex">
                                <div class="info-image me-3">
                                    <img class="p-3" src="../../../public/img/icon-3.png" alt="icon-1">
                                </div>
                                <div class="info-text">
                                    <h5 class="text-white">240K STREAMS COMPLETE</h5>
                                    <p>Distinctively provide acces mutfuncto users whereas communicate leveraged services</p>
                                </div>
                            </div>
                        </div>
                    </div> 
                </div>
            </div>
        </div>

    </section>
    
</template>

<style lang="scss" scoped>
@use '../../scss/partials/vars' as *;
    .game-collections{
        background-color: darken($color_blue, $amount: 10%);
        .top{
            .mc-card{
            width: calc(100% / 3 - 20px);
            height: 250px;
            background-color: #232A5C;
            margin-right: 10px;
            border-radius: 4px;

                &:last-child{
                    margin-right: -10px;
                }
            }
        }
        .line{
            border-bottom: 1px solid #21274B;
            margin: 100px 0;
        }

        
        .bottom{
            .who-image{
                img{
                    width: 100%;
                }
            }

            .infos{
                .info{
                    .info-image{
                        img{
                            border-radius: 50%;
                            background-color: $color_red;
                        }
                    }

                    .info-text{
                        h5{
                            font-weight: 700;
                        }
                    }
                }
            }
        }
    }
</style>