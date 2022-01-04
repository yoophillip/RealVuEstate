<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <div>
      <h4>XX OneRoom</h4>
      <p>{{ price1 }} Dollar</p>
    </div>
    <div>
      <h4>XX OneRoom</h4>
      <p>{{ price2 }} Dollar</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      price1: 60,
      price2: 70,
    };
  },
  components: {},
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
