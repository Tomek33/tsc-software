<template>
  <div id="app">
    <div class="container-fluid my-container">
      <Layout></Layout>
    </div>
  </div>
</template>

<script>
import Layout from './components/Layout.vue';

export default {
  name: 'App',
  components: {
    Layout
  }
}
</script>

<style>
  .my-container{
    padding-left: 0px;
    padding-right: 0px;
  }
</style>
