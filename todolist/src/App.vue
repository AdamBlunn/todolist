<template>
  <div id="app">
    <to-dos v-bind:todos="todos"/>
  </div>
</template>

<script>
import ToDos from "./components/Todos.vue";
export default {
  name: "app",
  components: {
    ToDos
  },
  data() {
    return {
      todos: [
        {
          id: 1,
          Title: "To Do 1",
          completed: false
        },
        {
          id: 2,
          Title: "To Do 2",
          completed: true
        },
        {
          id: 3,
          Title: "To Do 3",
          completed: false
        }
      ]
    };
  }
};
</script>

<style>
</style>
