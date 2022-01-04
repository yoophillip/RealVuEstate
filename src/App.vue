<template>
  <div id="app">
    <div class="menu">
      <a v-for="item in menu" :key="item">{{ item }}</a>
    </div>
    <div>
      <h4 class="red" style="color: red">{{ products[0] }}</h4>
      <p>10 Dollar</p>
      <button @click="reportCount = reportCount[0] + 1">
        False Listing Report
      </button>
      <span>Report Count : {{ reportCount[0] }} </span>
    </div>
    <div>
      <h4>{{ products[1] }}</h4>
      <p>20 Dollar</p>
      <button @click="increase">False Listing Report</button>
      <span>Report Count : {{ reportCount[1] }} </span>
    </div>
    <div>
      <h4>{{ products[2] }}</h4>
      <p>30 Dollar</p>
      <button @click="increase">False Listing Report</button>
      <span>Report Count : {{ reportCount[2] }} </span>
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
      reportCount: [0, 0, 0],
    };
  },
  // methods: {
  //   increase() {
  //     this.reportCount++;
  //   },
  // },
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
