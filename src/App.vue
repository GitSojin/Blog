<template>
  <List :blogText="blogText" />

</template>

<script>
import blog from "./assets/blog";
import List from "./components/List.vue";
export default {
  name: "App",
  components: { List },
  data() {
    return { blogText: blog };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
