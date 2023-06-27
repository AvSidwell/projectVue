<template>
    <div class="footer">
        <h6> Footer</h6>
        <p>
            <router-link class="menu" to="/">Home</router-link>
            <router-link class="menu" to="/">Tutorials</router-link>
            <router-link class="menu" to="/'">About</router-link>
        </p>
    </div>
</template>

<script>
    export default {

    }
</script>
<style>
 .footer {
    position: fixed;
    left: 0;
    bottom: 0;
    height: 5rem;
    width: 100%;
    background-color: rgb(61, 61, 61);
    overflow: hidden;
    text-align: center;
    padding: 0.7rem;
    /* height: 3rem; */
}

.menu {
    text-decoration: none;
    flex-direction: column;
    color: rgb(162, 162, 162);
    text-align: center;
    margin: 1rem;
    margin-left: 20px;
    font-size: x-large;
    /* text-decoration: none; */
}


.menu:hover {
    background-color: rgb(162, 162, 162);
    color: rgb(61, 61, 61);
    border-radius: 0.2rem;
}
</style>