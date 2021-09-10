<template>
  <div id="app">
    <HomePage />
  </div>
</template>

<script>
import HomePage from "./components/homePage.vue";

export default {
  name: "App",
  components: {
    HomePage,
  },
};
</script>

<style>
* {
  padding: 0;
  margin: 0;
}
body {
  /* width: 1920px; */
}
/* @font-face {
  font-family: Microsoft YaHei;
  src: url("./assets/微软雅黑/msyhl.ttc");
} */
</style>
