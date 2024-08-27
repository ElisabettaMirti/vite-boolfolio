<script>
export default {
    data(){
        return {

        }
    }
}

</script>

<template>
<header>
    <nav class="navbar-nav">
        <ul>
            <li>
                Home
            </li>
            <li>
                Project List
            </li>
            <li>
                About
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

ul{
    list-style-type: none;
    display: flex;
    justify-content: center;
    align-items: center;

    li{
        padding: 1rem;
        margin-top: 1rem;
    }
}

</style>
