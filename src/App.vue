<template>
  <Header/>
  <Main msg="Welcome to Your Vue.js App"/>
</template>

<script>
import Main from './components/Main.vue'
import Header from './components/Header.vue'

// eslint-disable-next-line no-undef

export default {
  name: 'App',
  components: {
    Main,
    Header
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
<style>
@font-face {
  font-family: "Inter";
  src: local("Inter"),
  url(./fonts/Inter-VariableFont_slnt,wght.ttf) format("truetype");
}
</style>
