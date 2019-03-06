<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <Base title="Base"/>
    <router-view></router-view>
  </div>
</template>

<script>
import Base from '@/components/Base.vue'

import Style from './assets/style.css'

export default {
  name: 'app',
  components: {
    'Base':Base,
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
