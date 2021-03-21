<template>
  <div>
    <child :n="n" @add:n="n += 1" @reduce:n="n -= 1" @reset:n="n = 0" />
  </div>
</template>

<script>
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