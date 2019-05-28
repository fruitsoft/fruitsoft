<template>
  <div id="app">
    <intro />
    <div id="container">
      <navBar id="nav" />
      <router-view id="view" />
    </div>
    <copyright />
  </div>
</template>

<script>
import intro from "@/components/intro";
import copyright from "@/components/copyright";
import navBar from "@/components/nav";

export default {
  components: {
    navBar,
    intro,
    copyright
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
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: #212931;
}
</style>

<style scoped>
#container {
}

#nav {
}

#view {
}
</style>
