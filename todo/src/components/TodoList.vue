<template>
  <ul id="todo-list">
    <li
      v-for="todo in todoList"
      :key="todo.id"
      :class="{ completed: todo.completed }"
    >
      {{ todo.msg }}
      Sample Task 1
      <button type="button" @click="todoUpdate(todo.id)">Delete</button>
    </li>
  </ul>
</template>

<script>
export default {
  props: ["todoList"],
  methods: {
    todoUpdate(id) {
      this.$emit("todoUpdate", id);
    },
  },
};
</script>
