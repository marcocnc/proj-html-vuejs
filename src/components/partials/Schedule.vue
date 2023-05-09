
<script>
export default {
    name: 'Schedule'
}
</script>

<template>
    <section class="schedule text-white pt-5">
        <div class="container d-flex flex-column justify-content-center align-items-center">
            <h5>titolo</h5>
            <h3>Titolo</h3>

            <!-- Main Match -->
            <div class="main-match w-100 my-4">
                <h2 class="border text-center">Main Match</h2>
            </div>

            <!-- All Matches -->
            <div class="all-matches d-flex w-100">

                <!-- Upcoming -->
                <div class="upcoming d-flex flex-column w-50">
                    <h1>Titolo</h1>
                    <h2>up</h2>
                    <h2>up</h2>
                    <h2>up</h2>
                </div>

                <!-- Previous -->
                <div class="previous d-flex flex-column w-50">
                    <h1>Titolo</h1>
                    <h2>prev</h2>
                    <h2>prev</h2>
                    <h2>prev</h2>
                </div>
            </div>

            <button class="btn btn-primary mt-5">BOTTONE</button>
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
    }
</style>