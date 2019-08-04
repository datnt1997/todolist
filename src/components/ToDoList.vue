
<template>
  <div class="hello">
    <h1 v-blind:title="message">{{ msg }}</h1>
    <ToDoItem />
  </div>
</template>

<script>
import ToDoItem from "./ToDoItem.vue";
export default {
  name: "ToDoList",
  components: {
    ToDoItem
  },
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
