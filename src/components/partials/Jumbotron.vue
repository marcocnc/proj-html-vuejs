
<script>
export default {
    name:'Jumbotron'
}
</script>

<template>
  
    <section id="jumbotron">

        <div class="mc-container h-100 text-white d-flex justify-content-start align-items-center">
            <div class="text">
                <h1>TITOLO</h1>
                <h2>TITOLO</h2>
                <p>Desc</p>
                <button class="btn btn-primary text-white">button</button>
            </div>
        </div>
    </section>
</template>

<style lang="scss" scoped>
    #jumbotron{
        height: 700px;
        background: #000000a1;
        background-image: url(../../../public/img/bg.jpg);
        background-position: center;

        h1{
            font-size: 100px;
        }
    }
</style>