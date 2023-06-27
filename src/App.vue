<template>
  <nav>
    <!-- <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> -->
<NavBarComp/>
<FooterComp/>
<FormView/>
  </nav>
  <router-view/>
</template>

<script>
  import NavBarComp from './components/Nav-Bar-View.vue';
  import FooterComp from './components/Footer-View.vue';
  import FormView from './components/Footer-View.vue';
  export default {
    components: {NavBarComp, FooterComp, FormView }
  }
</script>

<!-- 
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style> -->
