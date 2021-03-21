<template>
  <div>
    <h3>子组件的n：{{ n }}</h3>
    <h3>子组件按钮：</h3>
    <button @click="add">n+1</button>
    <button @click="reduce">n-1</button>
    <button @click="reset">reset</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      n: 0,
    };
  },
  methods: {
    add() {
      this.n += 1;
      this.$emit('add:n', this.n);
    },
    reduce() {
      this.n -= 1;
      this.$emit('reduce:n', this.n);
    },
    reset() {
      this.n = 0;
      this.$emit('reset:n', this.n);
    },
  },
};
</script>