<template>
  <div id="app">
    <Header/>
  </div>
</template>

<script>
import Header from './components/Header.vue'

export default {
  components: { Header },
  name: 'App'
}
</script>

<style lang="scss">
#app {
  background-color: $dark-blue;
  min-height: 100vh;
  color: white;
  font-family: 'Open Sans', sans-serif;
}
</style>
