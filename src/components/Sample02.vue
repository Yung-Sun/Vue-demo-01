<template>
  <div>
    <h2>父组件向子组件传值</h2>
    <father />
  </div>
</template>

<script>
import father from './02-father.vue';
export default {
  components: { father },
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