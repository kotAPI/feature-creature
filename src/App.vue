<template>
  <div id="app">
    <FeatureEditTable />
  </div>
</template>

<script>
import FeatureEditTable from "./components/FeatureEditTable.vue";

export default {
  name: "app",
  components: {
    FeatureEditTable
  },
  data() {
    return {};
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
