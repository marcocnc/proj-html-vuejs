<script>
export default {
    name: 'LiveStreamings'
}
</script>

<template>
    <section class="live-streamings pt-5">
        <div class="mc-container">
            <div class="titles text-center pt-5">
                <h5>titolo</h5>
                <h3 class="pb-3">Titolo</h3>
            </div> 
            
                <!-- Row with 2 cols -->
                <div class="row">
                    
                    <div class="col-6 p-2">
                        <div class="video border">
                            <div class="play d-flex justify-content-end flex-column align-items-center h-50">
                                <span>Play</span>
                            </div>
                            <div class="video-content text-start p-5">
                                <button class="btn btn-primary">bottone</button>
                                <h2 class="pt-2">TITOLO VIDEO</h2>
                            </div>
                        </div>
                    </div>
                    
                    <div class="col-6 p-2">
                        <div class="video border">
                            <div class="play d-flex justify-content-end flex-column align-items-center h-50">
                                <span>Play</span>
                            </div>
                            <div class="video-content text-start p-5">
                                <button class="btn btn-primary">bottone</button>
                                <h2 class="pt-2">TITOLO VIDEO</h2>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Row with 3 cols -->
                <div class="row">

                    <div class="col-4 p-2">
                        <div class="video border">
                            <div class="play d-flex justify-content-end flex-column align-items-center h-50">
                                <span>Play</span>
                            </div>
                            <div class="video-content text-start p-5">
                                <button class="btn btn-primary">bottone</button>
                                <h2 class="pt-2">TITOLO VIDEO</h2>
                            </div>
                        </div>
                    </div>

                    <div class="col-4 p-2">
                        <div class="video border">
                            <div class="play d-flex justify-content-end flex-column align-items-center h-50">
                                <span>Play</span>
                            </div>
                            <div class="video-content text-start p-5">
                                <button class="btn btn-primary">bottone</button>
                                <h2 class="pt-2">TITOLO VIDEO</h2>
                            </div>
                        </div>
                    </div>

                    <div class="col-4 p-2">
                        <div class="video border">
                            <div class="play d-flex justify-content-end flex-column align-items-center h-50">
                                <span>Play</span>
                            </div>
                            <div class="video-content text-start p-5">
                                <button class="btn btn-primary">bottone</button>
                                <h2 class="pt-2">TITOLO VIDEO</h2>
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
        padding-bottom: 120px;

        .col-6,
        .col-4{
            height: 350px;
        }

        .video{
            height: 100%;

            
        }
    }
</style>