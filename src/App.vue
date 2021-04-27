<template>
  <div id="app">
    <Header/>
    <div class="container-fluid">
      <div class="row justify-content-between">
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
    <div class="container-fluid my-3">
      <div class="row  align-items-between">
        <div class="col">
           <Card theme="water_level"/>
        </div>
        <div class="col">
            <div class="contents">
              <Irrigation/>
              <Ventilation/>
            </div>
        </div>
        <div class="col-6">

        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Card from './components/Card.vue'
import Irrigation from './components/Irrigation.vue'
import Ventilation from './components/Ventilation.vue'

export default {
  components: { Header, Card, Irrigation, Ventilation },
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
.contents{
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 250px;

}
</style>
