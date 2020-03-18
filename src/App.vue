<template>
  <div id="app">
    {{msg}}
    <div>
      <input type="text" v-model="info">
      <button v-on:click="handleClick">添加</button>
    </div>
    <ul>
      <todo-item v-for="item in list" v-bind:item="item"></todo-item>
    </ul>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
  }
}
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
