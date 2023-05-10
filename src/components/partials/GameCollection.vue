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
                    testo
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
            border-bottom: 1px solid white;
            margin: 100px 0;
        }

        .mc-buttons {
            box-shadow: 4px 4px $color_red;
            i{
                color: $color_white;
                background-color: $color_red;
                border-radius: 50%;
                padding: 1px 2px;
            }

            &:hover{
              background-color: $color_red;
              box-shadow: -4px -4px $color_white;
              transition: all .3s;
              color: $color_white;
            }

            &:hover i{
                color: $color_red;
                background-color: $color_white;
            }
        }
        .bottom{
            .who-image{
                img{
                    width: 100%;
                }
            }

            .who-text{
                background-color: #a24d4db6;
            }
        }
    }
</style>