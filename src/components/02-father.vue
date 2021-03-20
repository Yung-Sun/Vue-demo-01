<template>
  <div>
    <h3>父组件按钮：</h3>
    <button @click="add">n+1</button>
    <button @click="reduce">n-1</button>
    <button @click="reset">reset</button>
    <child :n="n" />
  </div>
</template>

script <script>
import child from './02-child.vue';
export default {
  components: { child },
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