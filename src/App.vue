<template>
  <div id="app">
    <Merge />
  </div>
</template>

<script>
import Merge from "./components/Merge.vue";

export default {
  name: "app",
  components: {
    Merge,
  },
  created() {},
  mounted() {},
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
