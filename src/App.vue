<template>
  <div id="app">
    <div class="menu">
      <a v-for="item in menu" :key="item">{{ item }}</a>
    </div>
    <div v-for="item in products" :key="item">
      {{ item }}
    </div>
    <div>
      <h4>{{ products[1] }}</h4>
      <p>20 Dollar</p>
    </div>
    <div>
      <h4>{{ products[2] }}</h4>
      <p>30 Dollar</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      price1: 10,
      price2: 70,
      products: ["NYC", "Chicago", "LA"],
      menu: ["Home", "Shop", "About"],
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
}

.menu {
  background: darkslateblue;
  padding: 15px;
  border-radius: 5px;
}

.menu a {
  color: white;
  padding: 10px;
}
</style>
