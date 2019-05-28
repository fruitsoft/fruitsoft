<template>
  <nav id="nav">
    <div class="routes">
      <router-link to="/" exact>Inicio</router-link>
      <router-link to="/productos">Productos</router-link>
      <router-link to="/documentos" @click="alert('Contenido no disponible')"
        >Documentos</router-link
      >
      <router-link to="/licencias">licecias</router-link>
      <router-link to="/contacto">Contacto</router-link>
    </div>
    <div class="social">
      <font-awesome-icon icon="twitter" />
      <font-awesome-icon icon="facebook" />
      <font-awesome-icon icon="instagram" />
      <font-awesome-icon icon="github" />
    </div>
  </nav>
</template>

<script>
export default {
  name: "navBar"
};
</script>

<style scoped>
#nav {
  display: flex;
  height: 58px;
  line-height: 58px;
  background-color: rgba(255, 255, 255, 0.176);
  text-transform: uppercase;
  font-size: 12px;
  font-weight: 900;
  flex-direction: row;
  justify-content: space-between;
}

.routes {
}

.social {
}

a {
  display: inline-block;
  vertical-align: middle;
  height: 58px;
  padding: 0 30px;
  text-decoration: none;
}

.router-link-active {
  background-color: #fff;
  color: #1e252d !important;
}
</style>
