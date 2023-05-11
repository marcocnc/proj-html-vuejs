<script>
export default {
    name: 'Loading'
}
</script>

<template>
    <div class="loading-layer d-flex justify-content-center align-items-center">
        <div class="lds-ripple"><div></div><div></div></div>
    </div>
</template>

<style lang="scss" scoped>
@use '../../scss/partials/vars' as *;

    .loading-layer{
        height: 100vh;
        background-color: $color_red;
        position: fixed;
        z-index: 999;
        width: 100%;
    }
    .lds-ripple {
        display: inline-block;
        position: relative;
        width: 80px;
        height: 80px;
    }
    .lds-ripple div {
        position: absolute;
        border: 4px solid #fff;
        opacity: 1;
        border-radius: 50%;
        animation: lds-ripple 1s cubic-bezier(0, 0.2, 0.8, 1) infinite;
    }
    .lds-ripple div:nth-child(2) {
        animation-delay: -0.5s;
    }

    @keyframes lds-ripple {
    0% {
        top: 36px;
        left: 36px;
        width: 0;
        height: 0;
        opacity: 0;
    }
    4.9% {
        top: 36px;
        left: 36px;
        width: 0;
        height: 0;
        opacity: 0;
    }
    5% {
        top: 36px;
        left: 36px;
        width: 0;
        height: 0;
        opacity: 1;
    }
    100% {
        top: 0px;
        left: 0px;
        width: 72px;
        height: 72px;
        opacity: 0;
    }
    }
</style>