<template>
  <div id="app">
    <Header/>
    <div class="container-fluid">
      <div class="row justify-content-center">
        <div class="col ">
          <Card theme="temperature"/>
        </div>
        <div class="col">
          <Card theme="humidity"/>
        </div>
        <div class="col">
          <Card theme="moisture"/>
        </div>
        <div class="col">
           <Card theme="ph"/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Card from './components/Card.vue'

export default {
  components: { Header, Card },
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
