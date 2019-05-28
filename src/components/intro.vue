<template>
  <div id="intro">
    <img src="@/assets/images/logot.png" width="100" />
    <h1>Fruitsoft</h1>
    <p>El socio de tu negocio</p>
    <ul class="actions">
      <li>
        <a href="#cabecera" class="button icon solo scrolly">
          <font-awesome-icon icon="arrow-down" />
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "intro"
};
</script>

<style scoped>
#intro {
  position: relative;
  min-height: 90vh;
  background-image: url(../assets/images/overlay.png),
    linear-gradient(0deg, rgba(0, 0, 0, 0.1), rgba(0, 0, 0, 0.1)),
    url(../assets/images/blue.jpg);
  background-size: auto, auto, 100% auto;
  background-position: center, center, top center;
  background-repeat: repeat, no-repeat, no-repeat;
  background-attachment: scroll, scroll, scroll;
  transition: opacity 1s ease, transform 1s ease;
}

.button.icon.solo.scrolly svg {
  position: absolute;
  height: 100%;
  transform: translateX(-50%);
  text-align: center;
  font-size: 2em;
}
</style>
