<template>
  <div>
    <h2>子组件显示父组件的值</h2>
    <strong>Props方法</strong>
    <p>
      data 在父组件中，button 和 methods 在父组件中，子组件只是显示
      data，不能改变
    </p>
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