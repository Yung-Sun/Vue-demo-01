<template>
  <div>
    <h3>Props传给子组件的n：{{ n }}</h3>
    <h3>子组件按钮：</h3>
    <button @click="add">n+1</button>
    <button @click="reduce">n-1</button>
    <button @click="reset">reset</button>
  </div>
</template>

<script>
export default {
  props: ['n'],
  methods: {
    add() {
      this.$emit('add');
    },
    reduce() {
      this.$emit('reduce');
    },
    reset() {
      this.$emit('reset');
    },
  },
};
</script>