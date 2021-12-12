<template>
  <div id="app">
    <Home/>
  </div>
</template>

<script>

import Home from "@/components/Home";
export default {
  name: 'App',
  components: {
    Home
  }
}
</script>

<style>
  body{
    margin: 0;
    background-color: #f2f2f2;
  }
  .container{
    align-items: center;
    max-width: 1200px;
    margin: auto;
  }
</style>
