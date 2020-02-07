<template>
  <div id="app">
    <div class="custom-input" @input="handleUserInput">
      <span style="color:green;">{{abc}}</span>
      <span>abc</span>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data: () => ({
    abc: "123"
  }),
  components: {},
  methods: {
    handleUserInput(event) {
      console.log(event.target.innerText);
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
.custom-input {
  -moz-user-modify: read-write;
  -webkit-user-modify: read-write;
}
</style>
