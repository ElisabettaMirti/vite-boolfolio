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
    <div class="card p-0 m-3">
        <img :src="project.url" alt="" class="card-img-top">
        <div class="card-body">
            <h5 class="card-title">{{project.title}}</h5>
            <p class="card-text"><em>Programming Languages: </em>{{ project.prog_langs }}</p>
            <!-- <a href="#" class="btn btn-primary">Go somewhere</a> -->
        </div>
    </div>

</template>

<style lang="scss">

div.card{
    width: 15rem;
}

</style>
