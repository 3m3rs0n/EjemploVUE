<template>
  <div id="app">
    <img alt="Vue logo" src="https://vuejs.org/images/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <ColorButton msg="Cambiar color" />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import ColorButton from './components/colorButton.vue';

export default {
  name: 'App',
  components: {
    HelloWorld,
    ColorButton,
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
