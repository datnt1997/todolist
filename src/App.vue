<template>
  <div id="app">
    <div class="container-fluid">
       <div class="row">
          <div class="col-md-6 offset-md-3">
            <ToDoList msg="Welcome to Your Vue.js App"/>
          </div>
       </div>
    </div>
  </div>
</template>

<script>
import ToDoList from './components/ToDoList.vue'

export default {
  name: 'app',
  components: {
    ToDoList
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
