<template>
  <div id="app">
    <hello></hello>
    <hr>
    <project-list></project-list>
  </div>
</template>

<script>
import Hello from './components/Hello'
import ProjectList from './components/ProjectList'

export default {
  name: 'app',
  components: { Hello,  ProjectList }
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
