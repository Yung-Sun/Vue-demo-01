<template>
  <div>
    <child :n="n" @add="n += 1" @reduce="n -= 1" @reset="n = 0" />
  </div>
</template>

script <script>
import child from './03-child.vue';
export default {
  components: { child },
  data() {
    return {
      n: 0,
    };
  },
};
</script>