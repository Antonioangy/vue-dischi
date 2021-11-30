<template>
  <div id="app">
    <Header/>
    <Type/>
    <Main/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Type from '@/components/Type.vue'
import Main from '@/components/Main.vue'
export default {
  name: 'App',
  components: {
    Header,
    Type,
    Main
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background-color: #1e2d3b;
}
body{
  margin: 0;
}
</style>
