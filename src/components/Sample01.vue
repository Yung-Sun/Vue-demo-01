<template>
  <div>
    <h3>n: {{ n }}</h3>
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
    },
    reduce() {
      this.n -= 1;
    },
    reset() {
      this.n = 0;
    },
  },
};
</script>