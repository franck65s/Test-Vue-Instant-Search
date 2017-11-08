<template>
  <ais-index
    app-id="latency"
    api-key="3d9875e51fbd20c7754e65422f7ce5e1"
    index-name="bestbuy"
  >
    <ais-search-box></ais-search-box>
    <ais-results>
      <template scope="{ result }">
        <h2>
          <ais-highlight :result="result" attribute-name="name"></ais-highlight>
        </h2>
      </template>
    </ais-results>
  </ais-index>
</template>

<script>
export default {
  name: 'app',
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
  text-align: center;
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
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
