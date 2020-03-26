<template>
  <div id="app">
    <button @click="click">Button</button>
    <p v-if="toggle">Toggle</p>
  </div>
</template>

<script>
export default {
  name: "App",
  data () {
    return {
      toggle: false
    }
  },
  methods: {
    click () {
      this.toggle = !this.toggle
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
