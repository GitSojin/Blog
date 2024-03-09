<template>
  <h1>Sojin Blog</h1>
  <router-link to="/home">홈페이지</router-link>
  <router-link to="/list">리스트페이지</router-link>
  <router-link to="/detail">상세페이지</router-link>
  <router-view :blogText="blogText"></router-view>
</template>

<script>
import blog from "./assets/blog";
export default {
  name: "App",
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
