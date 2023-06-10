<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <Food />
  <KeepAlive>
    <Beverage v-if="showBev" />
  </KeepAlive>
  <button @click="toggleBeverages">Show Beverages</button>
</template>

<script>
import Food from "./components/Food.vue";
import Beverage from "./components/Beverage.vue";
export default {
  name: "App",
  components: {
    Food,
    Beverage,
  },
  data() {
    return {
      showBev: false,
    };
  },
  methods: {
    toggleBeverages() {
      this.showBev = !this.showBev;
    },
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
