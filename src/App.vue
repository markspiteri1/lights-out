<template>
  <div id="app">
    <LightsOutGrid />
    <LightsOutCell :isOn="true" />
  </div>
</template>

<script>
import LightsOutGrid from "./components/LightsOutGrid.vue";
import LightsOutCell from "./components/LightsOutCell.vue";

export default {
  name: "App",
  components: {
    LightsOutGrid,
    LightsOutCell,
  },
};
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
