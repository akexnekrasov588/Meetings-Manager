<template>
  <div id="app">
    <h1> Fetch Data</h1>
    <WeeksList />
  </div>
</template>

<script>
  import WeeksList from './components/WeekList.vue'  

  export default {
    name: 'App',
    components: {
      WeeksList
    }
  }
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
