<template>
  <div id="app">
    <div class="lorem-class">{{ msg }}</div>
    <button v-on:click="clickHandler('value passed to clickHandler')">Click Me!</button>
  </div>
</template>

<script>
  export default {
    name: 'app',
    data () {
      return {
        msg: 'some test text'
      }
    },
    methods: {
      clickHandler(input) {
        return input + 1;
      }
    }
  }
</script>

<style>
  body {
    color: red;
  }
</style>
