
<script>
import Jumbotron from './partials/Jumbotron.vue';
import GameCollection from './partials/GameCollection.vue';
import Schedule from './partials/Schedule.vue';
import Squads from './partials/Squads.vue';
import LiveStreamings from './partials/LiveStreamings.vue';

export default {
    name:'Main',
    components:{
        Jumbotron,
        GameCollection,
        Schedule,
        Squads,
        LiveStreamings
    }
}
</script>

<template>
    <main>

        <Jumbotron />

        <GameCollection/>

        <Schedule />

        <Squads />

        <LiveStreamings/>
    </main>
</template>

<style lang="scss" scoped>
    
</style>