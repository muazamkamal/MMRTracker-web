<template>
  <div id="app">
    <GitHub/>
  </div>
</template>

<script>
import GitHub from './components/GitHub.vue'

export default {
  name: 'app',
  components: {
    GitHub
  }
}
</script>

<style>
html {
  margin: 0;
  padding: 0;

  height: 100vh;
  width: 100%;
}

body {
  background-color: rgb(14, 14, 14)
}
</style>
