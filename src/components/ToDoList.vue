
<template>
  <div class="hello">
    <div class="row">
      <div class="col-9">
        <input
          type="text"
          class="form-control"
          placeholder="Type your link"
          aria-label="Link"
          v-model="src"
          aria-describedby="basic-addon1"
        />
      </div>
      <div class="col-3">
        <button type="button" class="btn btn-primary">Add To List</button>
      </div>
    </div>
    <div class="row">
      <div class="col-10 offset-1 image">
        <img v-bind:src="src" />
      </div>
    </div>
    <!-- <ToDoItem /> -->
  </div>
</template>

<script>
import ToDoItem from "./ToDoItem.vue";
export default {
  name: "ToDoList",
  data: function () {
    return {
      src: ''
    }
  },
  components: {
    ToDoItem
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
.link-button {
  display: flex;
}
.image {
  margin-top: 20px;
}
.image img {
  max-width: 569px;
}
</style>
