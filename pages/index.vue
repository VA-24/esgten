<template>
  <div class="fullscreen">
    <link rel="stylesheet" href="styles.css">
    <div class="grad-bg absolute opacity-30">
      <div class="grad-bg bg-gradient-to-br from-grad_gray to-grad_blue"></div>
    </div>
    <sideBar></sideBar>
    <div id="app">
      <h1 class="hover:italic">To Do List</h1>
      <lineGraph></lineGraph> 
    </div>
  </div>
</template>

<script>
  // import * as d3 from "d3"
  import lineGraph from "../components/lineGraph.vue"
  import sideBar from "../components/sideBar.vue"

  export default {
    name: 'App',
    components: {
      lineGraph,
      sideBar
    },
  }


</script>


<style>
@tailwind base;
@tailwind components;
@tailwind utilities;

.fullscreen {
  height: 100vh;
  width: 100vw;
}

.grad-bg {
  text-align: right;
  width: 88vw;
  height: 100vh;
}

#app {
  width: 87vw;
  margin-left: 14vw;
}
</style>