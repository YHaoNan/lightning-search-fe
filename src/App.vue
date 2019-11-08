<template>
  <div id="app">
    <CenterLayout>
      <LeftLayout id="left-layout"></LeftLayout>
      <RightLayout id="right-layout"></RightLayout>
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

  @keyframes fadeInLeft{
    0%{
      transform: translateX(-100%);
      -webkit-transform: translateX(-100%);
      opacity: 0;
    }
    80%{
      transform: translateX(50%);
      -webkit-transform: translateX(0%);
      opacity: .8;
    }
    100%{
      transform: translateX(0%);
      -webkit-transform: translateX(0%);
      opacity: 1;
    }
  }


  @keyframes fadeInRight{
    0%{
      transform: translateX(100%);
      -webkit-transform: translateX(100%);
      opacity: 0;
    }
    80%{
      transform: translateX(50%);
      -webkit-transform: translateX(0%);
      opacity: .8;
    }
    100%{
      transform: translateX(0%);
      -webkit-transform: translateX(0%);
      opacity: 1;
    }
  }

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

#left-layout{
  -webkit-animation: fadeInLeft 1s;
  animation: fadeInLeft 1s;
}
#right-layout{
  -webkit-animation: fadeInRight 1s;
  animation: fadeInRight 1s;
}

</style>
