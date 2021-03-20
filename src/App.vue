<template>
  <div id="app">
    <h1>关于组件数据通信的demo</h1>
    <div class="sample01">
      <h2>组件内值变化</h2>
      <Sample01 />
    </div>
    <hr />
  </div>
</template>

<script>
import Sample01 from './components/Sample01.vue';
export default {
  name: 'App',
  components: { Sample01 },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.sample01 {
  text-align: left;
}
</style>
