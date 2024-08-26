<script>
import AppMain from './components/AppMain.vue';
import MainHeader from './components/MainHeader.vue';

export default {
    components:{
      MainHeader,
      AppMain
    }
}
</script>

<template>
  <MainHeader/>
  <AppMain/>
</template>

<style lang="scss"> 
@use "./styles/general.scss";
</style>
