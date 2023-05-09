<script>
export default {
    name: 'LiveStreamings'
}
</script>

<template>
    <section class="live-streamings py-5">
        <div class="mc-container">
            <div class="titles text-center pt-5">
                <h5>titolo</h5>
                <h3 class="pb-3">Titolo</h3>

                <!-- Row with 2 cols -->
                <div class="row">
                    
                    <div class="col-6 p-2">
                        <div class="video border">
                            <span>a</span>    
                        </div>
                    </div>
                    
                    <div class="col-6 p-2">
                        <div class="video border">
                            <span>a</span>
                        </div>
                    </div>
                </div>

                <!-- Row with 3 cols -->
                <div class="row">

                    <div class="col-4 p-2">
                        <div class="video border">
                            <span>a</span>
                        </div>
                    </div>

                    <div class="col-4 p-2">
                        <div class="video border">
                            <span>a</span>
                        </div>
                    </div>

                    <div class="col-4 p-2">
                        <div class="video border">
                            <span>a</span>
                        </div>
                    </div>
                </div>
            </div> 
        </div>
    </section>
</template>

<style lang="scss">
    .live-streamings{
        background-image: url('../../../public/img/bg\ \(3\).jpg');
        background-size: cover;
        background-attachment: fixed;

        .col-6,
        .col-4{
            height: 350px;
        }

        .video{
            height: 100%;
        }
    }
</style>