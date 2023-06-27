<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
    <FormView/>
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import FormView from '@/components/Form-View.vue'

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    FormView
}
}
</script>
