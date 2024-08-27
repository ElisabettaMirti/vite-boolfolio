<script>
import MainHeader from './components/MainHeader.vue';

export default {
    components:{
      MainHeader,
    }
}
</script>

<template>
  <MainHeader/>
  <router-view></router-view>
</template>

<style lang="scss"> 
@use "./styles/general.scss";
</style>
