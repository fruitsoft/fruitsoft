<template>
  <div id="app">
    <navBar />
    <router-view />
  </div>
</template>

<script>
import navBar from "@/components/nav";

export default {
  components: {
    navBar
  },
  beforeCreate() {
    alert(
      "Fruitsoft.mx se encuentra en face beta, las funciones se encuentran limitadas"
    );
  }
};
</script>

<style>
@import url(assets/css/main.css);
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
