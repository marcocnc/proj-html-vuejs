
<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';
import Loading from './components/partials/Loading.vue';
import {store} from './data/store';

export default {
    name:'App',
    components:{
      Header,
      Main,
      Footer,
      Loading
    },

    data(){
      return{
        store
      }
    },

    methods:{
      getImage(img){
        return new URL(img, import.meta.url).href;
      },

      stopLoading(){
        setInterval(() => {
          store.isLoading = false;
        }, 4000);
      }
    },

    mounted(){
      this.stopLoading();
    }
}
</script>

<template>
  <Loading v-if="store.isLoading"/>

    <Header />


    <Main />

    <Footer />
</template>

<style lang="scss">
@use './scss/main.scss' as *;
</style>