<template>
  <nav class="topNav">
    <router-link class="active" to="/">Home</router-link>
    <router-link to="/tutorials">Tutorials</router-link>
    <router-link to="/about">About</router-link>
  </nav>
</template>
<script>
    export default {

    } 

</script>
<style scoped>
.topNav {
    background-color: rgb(61, 61, 61);
    overflow: hidden;
    text-align: center;
    padding: 0.7rem;
    /* height: 3rem; */
}

.active {
    text-decoration: none;
    flex-direction: column;
    color: rgb(162, 162, 162);
    text-align: center;
    margin: 1rem;
    margin-left: 20px;
    font-size: x-large;
    /* text-decoration: none; */
}


.active:hover {
    background-color: rgb(162, 162, 162);
    color: rgb(61, 61, 61);
    border-radius: 0.2rem;
}
</style>