
<script>
import Jumbotron from './partials/Jumbotron.vue';
import GameCollection from './partials/GameCollection.vue';
import Schedule from './partials/Schedule.vue';
import Squads from './partials/Squads.vue';
import LiveStreamings from './partials/LiveStreamings.vue';
import Products from './partials/Products.vue';

export default {
    name:'Main',
    components:{
        Jumbotron,
        GameCollection,
        Schedule,
        Squads,
        LiveStreamings,
        Products
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

        <Products/>
    </main>
</template>

<style lang="scss" scoped>
    
</style>