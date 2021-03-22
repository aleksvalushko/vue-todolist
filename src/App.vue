<template>
  <div id="app">
    <h1>TodoList</h1>
    <hr />
    <todo-lists />
  </div>
</template>

<script>
import TodoLists from "./components/TodoLists";

export default {
  components: {
    TodoLists,
  },
};
</script>

<style lang="scss">
#app h1 {
  text-align: center;
}
</style>
