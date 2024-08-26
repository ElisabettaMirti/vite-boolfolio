<script>
export default {
    data(){
        return {

        }
    },
    props: [
        'project'
    ]
}

</script>

<template>
    <div class="card">
        <img :src="project.img_url" alt="" class="card-img-top">
        <div class="card-body">
            <h5 class="card-title">{{project.title}}</h5>
            <p class="card-text">Programming Languages: {{ project.prog_langs }}</p>
            <!-- <a href="#" class="btn btn-primary">Go somewhere</a> -->
        </div>
    </div>

</template>

<style lang="scss">

</style>
