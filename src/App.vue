<template>
  <main-page/>
</template>

<script>

import MainPage from "@/components/MainPage";
export default {
  name: 'App',
  components: {
    MainPage
  }
}
</script>

<style>

body {
  margin: 0;
  padding: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin: 0;
  padding: 0;
}
</style>
