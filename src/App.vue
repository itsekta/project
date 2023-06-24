<template>
  <NavBar/>
  <MainPage />
</template>

<script>
import NavBar from './components/NavBar.vue';
import MainPage from './components/MainPage.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    MainPage
  }
}
</script>

<style>
*,
*::before,
*::after {
  box-sizing: border-box;
  margin: 0px;
  padding: 0px;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #f5f8fa;
  height: 100vh;
}
</style>
