<template>
  <div id="app">
    <h1>TodoList</h1>
    <hr />
    <router-link to="/">Main page</router-link>
    <hr />
    <el-input placeholder="Your new task" v-model="input"></el-input>
    <hr />
    <todo-lists />
  </div>
</template>

<script>
import TodoLists from "./TodoLists";

export default {
  components: {
    TodoLists,
  },
  data() {
    return {
      input: "",
    };
  },
};
</script>

<style lang="scss">
#app h1 {
  text-align: center;
}
</style>
