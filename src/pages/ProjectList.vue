<script>
import AppMain from '../components/AppMain.vue';

export default {
    name: "ProjectList",
    components:{
        AppMain,
    }
}

</script>

<template>
    <h2>Project List</h2>
    <AppMain/>
</template>

<style lang="scss">
h2{
    color: rgb(217, 168, 217);
    text-align: center;
    margin-bottom: 2rem;
}
</style>
