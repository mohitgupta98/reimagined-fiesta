<template>
  <div id="app">
    <Header></Header>
    <div id="space_after_header"></div>
    <!-- <Homepage></Homepage> -->
    <!-- <Search></Search> -->
    <router-view/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
// import Search from './views/Search.vue'
// import Homepage from './views/Homepage.vue'
export default {
  components: { Header },
  name: 'App'
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#space_after_header{
  margin-bottom: 100px;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
