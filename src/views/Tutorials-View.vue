<template>
  <div v-if="tutorials" class="flex-conainer">
    <CardComp v-for="tutorial of tutorials" :key="tutorial.id" :tutorial="tutorial" />
  </div>
  <div v-else>Loading...</div>
</template>
<script>
import CardComp from "@/components/Card-Comp.vue";
export default {
  computed: {
    tutorials() {
      return this.$store.state.tutorials
    }
  },
  mounted() {
    this.$store.dispatch("getTutorials");
  },

  components: { CardComp },
}
</script>
