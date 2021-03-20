<template>
  <div>
    <h3>Props传给子组件的n：{{ n }}</h3>
  </div>
</template>

<script>
export default {
  props: ['n'],
};
</script>