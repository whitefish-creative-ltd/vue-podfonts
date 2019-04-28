<template>
  <div id="app">
    <PodfontIcon/>
  </div>
</template>

<script>
import PodfontIcon from "./components/PodfontIcon";

export default {
  name: "App",
  components: {
    PodfontIcon
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
