
<script>
export default {
    name:'Header'
}
</script>

<template>
  <header>

    <div class="container">
        <!-- Info -->
        <div class="header-info d-flex justify-content-between">

            <!-- Phone Number -->
            <div class="phone-number w-25">
                <span>numero</span>
            </div>

            <!-- Address -->
            <div class="address w-50">
                <span>Indirizzo</span>
            </div>

            <!-- Icons -->
            <div class="header-icons w-25">
                <span>icona</span>
                <span>icona</span>
                <span>icona</span>
                <span>icona</span>
                <span>icona</span>
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
                <div class="btn btn-primary text-white me-3">bottone</div>
                <div class="btn btn-primary text-white">bottone</div>
            </div>
        </div>  
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use '../scss/partials/vars' as *;

    header{
        background: $header_bgc;
        color:white;
    }

    .phone-number,
    .address,
    .header-icons{
        border-left: 1px solid white;
        border-right: 1px solid white;
        border-bottom: 1px solid white;
        padding: 10px;
    }

    .header-icons span{
        padding: 0 5px;
    }

    

</style>