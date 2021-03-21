<template>
  <div>
    <h2>父组件显示子组件的值</h2>
    <strong>$emit</strong>
    <p>
      data 在子组件中，button 和 methods
      在子组件中，子组件通过$emit发布事件并传值给父组件，父组件收到数据再更新n值。
    </p>

    <father />
  </div>
</template>

<script>
import father from './04-father.vue';
export default {
  components: { father },
};
</script>