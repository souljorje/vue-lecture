<template>
  <div id="app">
    <h2>Here go developers!</h2>
    <app-developers></app-developers>
  </div>
</template>

<script>
import Developers from './components/Developers/Developers'

export default {
  name: 'app',
  components: {
    'appDevelopers': Developers,
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: block;
  margin: 10px;
}

a {
  color: #42b983;
}
</style>
