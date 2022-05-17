<template>
  <div id="app">
    <HeaderMain title="Product page" />
    <ProductPage />
  </div>
</template>

<script>
import HeaderMain from './components/Header.vue'
import ProductPage from './components/ProductPage.vue'

export default {
  name: 'App',
  components: {
    HeaderMain,
    ProductPage
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
  margin: 0;
  padding: 0;
  background-color: #2c3e50;
}
</style>
