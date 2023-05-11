
<script>
import { headerLinks } from '../data/database'; 

export default {
    name:'Header',
    data(){
        return{
            headerLinks
        }
    }
}
</script>

<template>
  <header>

    <div class="mc-container">
        <!-- Info -->
        <div class="header-info d-flex justify-content-between">

            <!-- Phone Number -->
            <div class="phone-number w-25 p-3 text-center">
                <i class="fa-solid fa-phone"></i>
                <span>+800-123-4567 6587</span>
            </div>

            <!-- Address -->
            <div class="address w-50 p-3 ps-5">
                <i class="fa-solid fa-location-dot pe-2"></i>
                <span>Beverley, New York 224 USA</span>
            </div>

            <!-- Icons -->
            <div class="header-icons d-flex justify-content-between w-25">
                <a href="#" class="d-flex align-items-center pe-3">
                    <i class="fa-brands fa-facebook-messenger"></i>
                </a>

                <a href="#" class="d-flex align-items-center pe-3">
                    <i class="fa-brands fa-twitter"></i>
                </a>

                <a href="#" class="d-flex align-items-center pe-3">
                    <i class="fa-brands fa-vimeo-v"></i>
                </a>

                <a href="#" class="d-flex align-items-center pe-3">
                    <i class="fa-brands fa-skype"></i>
                </a>

                <a href="#" class="d-flex align-items-center pe-3">
                    <i class="fa-solid fa-rss rss"></i>
                </a>
            </div>
        </div>

        <!-- Main Menù -->

        <div class="header-mainmenu d-flex justify-content-between align-items-center pt-2">

            <!-- Logo -->
            <div class="logo">
                <img src="../../public/img/logo.png" alt="logo">
            </div>

            <!-- Navbar -->
            <nav>
                <ul class="d-flex align-items-center fw-bold">
                    <li v-for="(link, index) in headerLinks" :key="index">
                        <a href="#" class="pe-4 text-white">{{ link.text }}</a>
                    </li>
                </ul>
            </nav>

            <!-- Buttons -->
            <div class="buttons d-flex">
                <div class="header-btn">
                    <i class="fa-solid fa-user"></i>
                    <span class="ps-2">LOG IN</span>
                </div>
                <div class="header-btn-reverse">
                    <i class="fa-solid fa-users"></i>
                    <span class="ps-2">SIGN UP</span>
                </div>
            </div>
        </div>  
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use '../scss/partials/vars' as *;

    header{
        background: $header_bgc;
        font-family: 'Barlow', sans-serif;
    
        .phone-number,
        .header-icons{
            border-bottom: 1px solid #2D2E73;
        }
    
        .phone-number{
            border-right: 1px solid #2D2E73;
        }
        .address{
            border-bottom: 1px solid #2D2E73;
        }

        .phone-number i::before{
            content: "";
            position: absolute;
            height: 100px;
            top: -38px;
            margin-left: -96px;
            border-right: 1px solid #2D2E73;
            transform: rotate(-30deg);
        }

        .rss::after{
            content: "";
            position: absolute;
            height: 100px;
            top: -38px;
            margin-left: 42px;
            border-right: 1px solid #2D2E73;
            transform: rotate(30deg);
        }

        .header-icons a{
            color: $color_white;
            border-right: 1px solid #2D2E73;
            height: 100%;

            &:last-child{
                border: none;
            }
        }

        .header-mainmenu{
            ul{
                margin-bottom:0;
            }

            .header-btn,
            .header-btn-reverse{
                padding: 15px 10px;
                font-size: 15px;
            }

            .header-btn{
                background-color: $color_white;
                color: $color_red;
                box-shadow: 0 3px 0 0 $color_red;
            }

            .header-btn-reverse{
                background-color: $color_red;
                color: $color_white;
                box-shadow: 3px 3px 0 0 $color_white;
            }
        }
    }
</style>