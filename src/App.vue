<template>
  <div id="app">
    <img src="./assets/manager.png">
    <CashGrab/>
  </div>
</template>

<script>
import CashGrab from './components/CashGrab'

export default {
  name: 'app',
  components: {
    CashGrab
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
