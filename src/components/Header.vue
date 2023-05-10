
<script>
export default {
    name:'Header'
}
</script>

<template>
  <header>

    <div class="mc-container">
        <!-- Info -->
        <div class="header-info d-flex justify-content-between">

            <!-- Phone Number -->
            <div class="phone-number w-25 p-3 text-center">
                <i class="fa-solid fa-phone pe-2"></i>
                <span>+800-123-4567 6587</span>
            </div>

            <!-- Address -->
            <div class="address w-50 p-3">
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

        <div class="header-mainmenu d-flex justify-content-between pt-5">

            <!-- Logo -->
            <div class="logo">
                <span>IMMAGINE</span>
            </div>

            <!-- Navbar -->
            <nav>
                <span class="px-2">link</span>
                <span class="px-2">link</span>
                <span class="px-2">link</span>
                <span class="px-2">link</span>
                <span class="px-2">link</span>
            </nav>

            <!-- Buttons -->
            <div class="buttons">
                <div class="btn btn-primary me-3">bottone</div>
                <div class="btn btn-primary ">bottone</div>
            </div>
        </div>  
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use '../scss/partials/vars' as *;

    header{
        background: $header_bgc;
        
    
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
    }
</style>