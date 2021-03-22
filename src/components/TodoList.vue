<template>
  <el-row class="todolist">
    <span>
      <el-checkbox v-model="checked"></el-checkbox>
      <span>{{ index + 1 }}. </span>
    </span>
    <span>{{ todo.title }}</span>
    <el-button type="primary" icon="el-icon-delete"></el-button>
  </el-row>
</template>

<script>
export default {
  props: {
    todo: {
      type: Object,
      required: true,
    },
    index: {
      type: Number,
      required: true,
    },
  },
  data() {
    return {
      checked: false,
    };
  },
};
</script>

<style lang="scss">
.todolist {
  display: flex;
  justify-content: space-between;
}
</style>
