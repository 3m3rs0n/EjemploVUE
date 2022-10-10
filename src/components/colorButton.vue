<template>
  <button id="btn" v-on:click="setColor">{{ msg }}</button>
</template>

<script>
export default {
  name: 'ColorButton',
  props: {
    msg: String,
  },
  methods: {
    setColor: function (event) {
      const ColorsArray = [
        '#557588',
        '#4C8AB9',
        '#84C0F7',
        '#D0E9FB',
        '#91ce7b',
        'white',
      ];
      function cambiarColor() {
        const fondo = document.getElementById('fondo');
        var r = Math.floor(Math.random() * 6);
        fondo.style.backgroundColor = ColorsArray[r];
      }
      setInterval(function () {
        cambiarColor();
      }, 1000);
    },
  },
};
</script>

<style scoped>
button {
  width: 100px;
}
</style>
