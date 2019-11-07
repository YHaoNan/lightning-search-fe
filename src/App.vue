<template>
  <div id="app">
    <CenterLayout>
      <LeftLayout></LeftLayout>
      <RightLayout></RightLayout>
    </CenterLayout>
  </div>
</template>

<script>
import CenterLayout from "./components/CenterLayout.vue";
import LeftLayout from "./components/LeftLayout.vue";
import RightLayout from "./components/RightLayout.vue";

export default {
  name: 'app',
  components: {
    LeftLayout,
    CenterLayout,
    RightLayout
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
</style>
