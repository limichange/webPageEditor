<template>
  <div id="app">
    <main-nav></main-nav>
    <main-edit-area></main-edit-area>
  </div>
</template>

<script>
import MainNav from './components/MainNav.vue'
import MainEditArea from './components/MainEditArea.vue'

export default {
  name: 'app',
  components: {
    MainNav,
    MainEditArea
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
}
</style>
