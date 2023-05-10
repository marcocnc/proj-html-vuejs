
<script>
export default {
    name:'Footer'
}
</script>

<template>
    <footer>
        <div class="footer-top">

            <div class="mc-container">

                <!-- Row with phone, mail and address -->
                <div class="row">

                    <div class="col-4 p-4 phone">phone</div>

                    <div class="col-4 p-4 mail">mail</div>

                    <div class="col-4 p-4 address">address</div>

                </div>
            </div>
        </div>

        <!-- Footer center -->
        <div class="footer-center">
            <div class="mc-container">
                <div class="row">

                    <!-- Logo and Brands div -->
                    <div class="col-4 logo-brands">
                        <div class="logo">LOGO</div>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Exercitationem maiores minus tempora architecto, magni facere mollitia corporis pariatur eaque, aperiam vero illum aut adipisci aliquam dolor excepturi neque modi provident?</p>
                        <div class="brands d-flex">
                            <span>ICONA</span>
                            <span>ICONA</span>
                            <span>ICONA</span>
                        </div>
                    </div>

                    <!-- Teams div -->
                    <div class="col-4 jackpot">
                        <h3>Titolo</h3>
                        <div class="teams">

                            <!-- First team -->
                            <div class="team d-flex">
                                <div class="team-img">
                                    <img src="../../public/img/01 (4).jpg" alt="">
                                </div>
                                <div class="team-content ps-3">
                                    <h4>FREE POKER GAME</h4>
                                    <span>Poker: $230</span>
                                    <div class="stars">
                                        <span>icona</span>
                                        <span>icona</span>
                                        <span>icona</span>
                                        <span>icona</span>
                                        <span>icona</span>
                                    </div>
                                </div>
                            </div>

                            <!-- Second team -->
                            <div class="team d-flex mt-3">
                                <div class="team-img">
                                    <img src="../../public/img/01 (4).jpg" alt="">
                                </div>
                                <div class="team-content ps-3">
                                    <h4>FREE POKER GAME</h4>
                                    <span>Poker: $230</span>
                                    <div class="stars">
                                        <span>icona</span>
                                        <span>icona</span>
                                        <span>icona</span>
                                        <span>icona</span>
                                        <span>icona</span>
                                    </div>
                                </div>
                            </div>

                            <!-- Third team -->
                            <div class="team d-flex mt-3">
                                <div class="team-img">
                                    <img src="../../public/img/01 (4).jpg" alt="">
                                </div>
                                <div class="team-content ps-3">
                                    <h4>FREE POKER GAME</h4>
                                    <span>Poker: $230</span>
                                    <div class="stars">
                                        <span>icona</span>
                                        <span>icona</span>
                                        <span>icona</span>
                                        <span>icona</span>
                                        <span>icona</span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Newsletter -->
                    <div class="col-4 newsletter">
                        <h3>Titolo</h3>
                        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>

                        <input type="text" placeholder="Your name" class="p-2 w-100">
                        <input type="text" placeholder="Your email" class=" mt-4 p-2 w-100">

                        <button class="btn btn-primary mt-4">Bottone</button>
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
            border-bottom: 1px solid #fff;
            margin-bottom: 80px;

            .phone,
            .mail,
            .address{
                border-left: 1px solid #fff;
            }

            .address{
                border-right: 1px solid #fff;
            }
        }
        
    }
    .footer-bottom{
        height: 90px;
        background-color: $color_darkblue;
    }
</style>