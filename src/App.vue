<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <br />
    <button @click="exps++">⬆︎</button>
    <input v-model="exps" />
    <Degs :base="2" :exps="new Array(+exps).fill().map((e, i) => i + 10)" />
  </div>
</template>

<script>
import Degs from "./components/Degs.vue";

export default {
  name: "App",
  components: {
    Degs,
  },
  data() {
    return {
      exps: 3,
    };
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  padding-left: 100px;
  color: #2c3e50;
  margin-top: 60px;
}
button, input {
  zoom: 150%;
}
</style>
