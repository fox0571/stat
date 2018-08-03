<template>
  <div id="app">
    <Hello></Hello>
    <Hello></Hello>
    <Hello></Hello>
    <Hello></Hello>
  </div>
</template>

<script>
import Vue from 'vue'
import Element from 'element-ui'
import 'element-ui/lib/theme-chalk/index.css'
import Hello from './components/HelloWorld'
Vue.use(Element)
export default {
  name: 'app',
  components: {
    Hello
  },
  data: function () {
    return {
      active: true
    }
  },
  methods: {
    handleSelect (key, keyPath) {
      console.log(key, keyPath)
    }
  }
}
</script>

<style>
  body{margin: 0;}
  #app {
    min-width: 1200px;
    margin: 0 auto;
    font-family: "Helvetica Neue","PingFang SC",Arial,sans-serif;
  }

</style>
