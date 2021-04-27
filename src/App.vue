<template>
  <div id="app">
    <Header/>
    <div class="container-fluid">
      <div class="row mx-auto justify-content-center">
        <div class="col ">
          <Card>
            <template v-slot:title>
              <span class="banner">Temperature</span>
            </template>
            <template v-slot:warehouse>
              <p class="sub-title">Warehouse</p>
              <p class="value">25&#176;C</p>
            </template>
            <template v-slot:outside>
              <p class="sub-title">Outside</p>
              <p class="value">25&#176;C</p>
            </template>
          </Card>
        </div>
        <div class="col">
          <Card>
              <template v-slot:title>
                <span class="banner">Humidity</span>
              </template>
              <template v-slot:warehouse>
                <p class="sub-title">Warehouse</p>
                <p class="value">25&#176;C</p>
              </template>
              <template v-slot:outside>
                <p class="sub-title">Outside</p>
                <p class="value">25&#176;C</p>
              </template>
          </Card>
        </div>
        <div class="col">
          <Card>
            <template v-slot:title>
              <span class="banner">Moisture</span>
            </template>
            <template v-slot:warehouse>
              <p class="sub-title">Warehouse</p>
              <p class="value">25&#176;C</p>
            </template>
            <template v-slot:outside>
              <p class="sub-title">Outside</p>
              <p class="value">25&#176;C</p>
            </template>
          </Card>
        </div>
        <div class="col">
           <Card>
            <template v-slot:title>
              <span class="banner">Soil pH</span>
            </template>
            <template v-slot:warehouse>
              <p class="sub-title">Warehouse</p>
              <p class="value">25&#176;C</p>
            </template>
            <template v-slot:outside>
              <p class="sub-title">Outside</p>
              <p class="value">25&#176;C</p>
            </template>
          </Card>
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
