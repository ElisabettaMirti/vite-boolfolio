<script>
import axios from 'axios';
import ProjectCard from './ProjectCard.vue';

export default {
    data(){
        return {
            projects : [],
        }
    },
    components: {
        ProjectCard
    },
    methods: {
        getProjects(){
            axios.get('http://127.0.0.1:8000/api/projects', {
                params: {
                
                }
            })
            .then((response) => {
                console.log(response.data.results);
                this.projects = response.data.results; 
            })
            .catch(function (error) {
                console.log(error);
            })
            .finally(function () {
                // always executed
            });
        }
    },
    created(){
        this.getProjects();
    }
}

</script>

<template>
    <div class="container">
        <div class="row d-flex">
            <ProjectCard class="col-3" v-for="project in projects" :project="project"/>
        </div>
    </div>
</template>

<style>
div.row{
    flex-direction: row;
    justify-content: center;
}
</style>
