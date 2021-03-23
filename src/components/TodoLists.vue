<template>
  <div class="todolists">
    <todo-list
      v-for="(todo, index) in todolists"
      :todo="todo"
      :index="index"
      :key="index"
    />
  </div>
</template>

<script>
import TodoList from "./TodoList";

export default {
  components: {
    TodoList,
  },
  data() {
    return {
      todolists: [
        { id: 1, title: "One" },
        { id: 2, title: "Two" },
        { id: 3, title: "Three" },
      ],
    };
  },
};
</script>

<style lang="scss">
.todolists {
}
</style>
