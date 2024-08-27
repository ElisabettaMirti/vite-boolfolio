<script>
import { RouterLink } from 'vue-router';

export default {
    data(){
        return {
            navLinks : [
                {
                    label: "Home",
                    name: "home",
                },
                {
                    label: "Project List",
                    name: "projects",
                },
                {
                    label: "About",
                    name: "about"
                }               
            ]
        }
    }
}

</script>

<template>
<header>
    <nav class="navbar-nav">
        <ul class="nav">
            <li v-for="navItem in navLinks">
                <router-link :to="{ name: navItem.name }">
                    {{ navItem.label }}
                </router-link>
            </li>
        </ul>
    </nav>
</header>
</template>

<style lang="scss">

header{
    background-color: rgb(217, 168, 217);
    color: whitesmoke;
    margin-bottom: 2rem;
}

ul.nav{
    list-style-type: none;
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 1rem;

    li{
        padding: 1rem;


        a{
            color: white;
            text-decoration: none;
        }
    }
}

</style>
