<template>
    <router-link class="router" :to="{name: 'tutorial', params: {id: tutorial.id}}">
    <img :src="tutorial.image_url" :alt="tutorial.title">
    <h3>{{ tutorial.title }}</h3>
    <p>Description: {{ tutorial.desc }}</p>
    <p>Price: R {{ tutorial.price }}</p>
    </router-link>
</template>

<script>
    export default {
        props: ["tutorial"]
    }

</script>
 <style>

.router{
    width: 23rem;
    height: 23rem;
}

img {
    width: 100%;
    height: 23REM;
}

</style>