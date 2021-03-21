<template>
  <div>
    <child @add:n="fetch" @reduce:n="fetch" @reset:n="fetch" />
    <h3>父组件的n：{{ n }}</h3>
  </div>
</template>

<script>
import child from './04-child.vue';
export default {
  components: { child },
  data() {
    return {
      n: 0,
    };
  },
  methods: {
    fetch(n) {
      this.n = n;
    },
  },
};
</script>