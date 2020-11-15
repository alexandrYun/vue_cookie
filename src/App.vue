<template>
  <div id="app">
    <Cookie v-on:click="counterUp" />
    <h3>{{counter}}</h3>
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
      console.log('123')
    }
  }
}
</script>

<style>

</style>
