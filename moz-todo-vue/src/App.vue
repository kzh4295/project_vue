<template>
  <div id="app">
    <h1>To-DO List</h1>
    <todo-item label="jh"></todo-item>
  </div>
</template>

<script>
import ToDoItem from './components/TodoItem.vue';

export default {
  name: 'App',
  components: {
    'todo-item':ToDoItem,
  }
}
</script>

<style>
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */
</style>
