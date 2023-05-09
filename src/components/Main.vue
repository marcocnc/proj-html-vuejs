
<script>
import Jumbotron from './partials/Jumbotron.vue';
import GameCollection from './partials/GameCollection.vue';
export default {
    name:'Main',
    components:{
        Jumbotron,
        GameCollection
    }
}
</script>

<template>
    <main>
        <Jumbotron />

        <GameCollection/>
    </main>
</template>

<style lang="scss" scoped>
    
</style>