<template>
  <div class="todolist">
    <span class="number-block">
      <el-checkbox v-model="checked"></el-checkbox>
      <span>{{ index + 1 }}. </span>
    </span>
    <span>{{ todo.title }}</span>
    <el-button
      type="danger"
      icon="el-icon-delete"
      class="delete-btn"
    ></el-button>
  </div>
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
  align-items: center;
  padding: 2px 10px;
  max-width: 100%;
  border: 1px solid gray;
  margin: 5px;
}

.number-block {
  width: 2.5%;
  display: flex;
  justify-content: space-between;
}
</style>
