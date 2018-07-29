<template>
  <div id="app">
    <el-switch
      v-model="value2"
      active-color="#13ce66"
      inactive-color="#ff4949">
    </el-switch>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      value2: true
    };
  },
  watch: {
    value2(newValue) {
      console.log(newValue);
    }
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
