<template>
  <div id="app" class="wrapper">
    <Cookie v-on:counterup="counterUp" />
    <h3 class="counter">Печенек поймано: {{counter}}</h3>
  </div>
</template>

<script>
import Cookie from '@/components/Cookie'
export default {
  name: 'App',
  data() {
    return {
      counter: 0
    }
  },
  components: {
    Cookie
  },
  methods: {
    counterUp() {
      this.counter += 1
    }
  }
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Roboto:ital,wght@0,500;1,300&display=swap');

  .wrapper {
    width: 90%;
    margin: 20px auto;
    display: flex;
    flex-direction: column;
    align-items: center;
    font-family: 'Roboto', sans-serif;
  }
  .counter {
    font-weight: 300;
  }
</style>
