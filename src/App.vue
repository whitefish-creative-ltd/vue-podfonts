<template>
  <div id="app">
    <PodfontIcon/>
    <PodfontIconCSS icon="pocket-casts"/>
    <PodfontIconCSS host icon="blubrry" size="5x"/>
  </div>
</template>

<script>
import PodfontIcon from './components/PodfontIcon'
import PodfontIconCSS from './components/PodfontIconCSS'
export default {
  name: 'App',
  components: {
    PodfontIcon,
    PodfontIconCSS
  }
}
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin-top: 60px;
}
</style>
