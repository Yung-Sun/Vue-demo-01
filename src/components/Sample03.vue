<template>
  <div>
    <h2>子组件向父组件传值</h2>
    <strong>$emit</strong>
    <p>
      data 在父组件中，button 和 methods
      在子组件中，子组件通过$emit发布一个事件，父组件监听这个事件，修改n的值。
    </p>
    <p>可以理解成子组件的button通知父组件修改n值</p>
    <father />
  </div>
</template>

<script>
import father from './03-father.vue';
export default {
  components: { father },
};
</script>