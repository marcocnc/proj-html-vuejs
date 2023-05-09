<script>
export default {
    name:'GameCollection'
}
</script>

<template>
    
    <!-- Our Game Collections -->
    <section class="game-collections">

        <div class="mc-container">
            <div class="top d-flex flex-column justify-content-center align-items-center pt-5">
                <h5>titolo</h5>
                <h3>Titolo</h3>

                <!-- Cards -->
                <div class="mc-cards-container w-100 d-flex mt-4">
                    <div class="mc-card">Card</div>
                    <div class="mc-card">Card</div>
                    <div class="mc-card">Card</div>
                </div>

                <div class="game-coll-button btn btn-primary my-5">Bottone</div>
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
            border: 1px solid white;
            width: calc(100% / 3);
            margin-right: 10px;

                &:last-child{
                    margin-right: -10px;
                }
            }

        }
        .line{
            border-bottom: 1px solid white;
            margin: 100px 0;
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