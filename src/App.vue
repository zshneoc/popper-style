<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <common-table />

</template>

<script>
import CommonTable from './components/CommonTable.vue';

export default {
  name: 'App',
  components: {
    CommonTable
  }
}
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
</style>
