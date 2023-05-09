
<script>
import Jumbotron from './partials/Jumbotron.vue';
import GameCollection from './partials/GameCollection.vue';
import Schedule from './partials/Schedule.vue';
import Squads from './partials/Squads.vue';


export default {
    name:'Main',
    components:{
        Jumbotron,
        GameCollection,
        Schedule,
        Squads
    }
}
</script>

<template>
    <main>

        <Jumbotron />

        <GameCollection/>

        <Schedule />

        <Squads />

    </main>
</template>

<style lang="scss" scoped>
    
</style>