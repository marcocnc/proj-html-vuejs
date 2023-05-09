
<script>
import Jumbotron from './partials/Jumbotron.vue';
import GameCollection from './partials/GameCollection.vue';
import Schedule from './partials/Schedule.vue';
export default {
    name:'Main',
    components:{
        Jumbotron,
        GameCollection,
        Schedule
    }
}
</script>

<template>
    <main>
        
        <Jumbotron />

        <GameCollection/>

        <Schedule />

    </main>
</template>

<style lang="scss" scoped>
    
</style>