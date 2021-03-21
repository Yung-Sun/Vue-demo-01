<template>
  <div id="app">
    <h1>关于组件数据通信的demo</h1>
    <div class="sample 01">
      <h1>Sample 01</h1>
      <Sample01 />
    </div>
    <hr />
    <div class="sample 02">
      <h1>Sample 02</h1>
      <Sample02 />
    </div>
    <hr />
    <div class="sample 03">
      <h1>Sample 03</h1>
      <Sample03 />
    </div>
    <hr />
    <div class="sample 04">
      <h1>Sample 04</h1>
      <Sample04 />
    </div>
    <hr />
  </div>
</template>

<script>
import Sample01 from './components/Sample01.vue';
import Sample02 from './components/Sample02.vue';
import Sample03 from './components/Sample03.vue';
import Sample04 from './components/Sample04.vue';

export default {
  name: 'App',
  components: { Sample01, Sample02, Sample03, Sample04 },
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
.sample {
  text-align: left;
}
</style>
