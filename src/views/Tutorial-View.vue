<template>
  <div v-if="tutorial" class="tutorial-details">
    <img :src="tutorial.image_url" :alt="tutorial.title" />
    <div class="div">
      <h2>{{ tutorial.title }}</h2>
      <p class="paragraph">Description: {{ tutorial.decs }}</p>
      <p>Rating: {{ tutorial.rating }}</p>
    </div>
  </div>
</template>
<script>
export default {
  props: ["id"],
  computed: {
    tutorial() {
      return this.$store.state.tutorial;
    },
  },
  mounted() {
    this.$store.dispatch("getTutorial", this.id);
  },
};
</script>
<style>
.tutorial-details {
  margin: auto;
  margin-top: 2rem;
  width: 20rem;
}

.div {
  position: relative;
  animation-name: example;
  animation-delay: 3s;
  animation-duration: 2s;
}

@keyframes example {
  0% {
    right: 400px;
    top: 0px;
  }
  25% {
    right: 300px;
    top: 0px;
  }
  50% {
   right: 200px;
    top: 0px;
  }
  75% {
    right: 100px;
    top: 0px;
  }
  100% {
    right: 0px;
    top: 0px;
  }
}
.tutorial-details {
  position: relative;
  animation-name: examples;
  animation-delay: 3s;
  animation-duration: 2s;
}

@keyframes examples {
  0% {
    left: 400px;
    top: 0px;
  }
  25% {
    left: 300px;
    top: 0px;
  }
  50% {
    left: 200px;
    top: 0px;
  }
  75% {
    left: 100px;
    top: 0px;
  }
  100% {
    left: 0px;
    top: 0px;
  }
}

img {
  width: 100%;
  height: 20rem;
  margin: 0;
}
.div {
  text-align: center;
  margin: 0;
  border: solid;
  border-top: none;
}

h2 {
  color: white;
  background-color: black;
}

.paragraph {
  border-bottom: solid 1px;
}
</style>
