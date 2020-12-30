<template>
  <div id="app">
<!--    <navigation></navigation>-->
    <PageWithProducts
      v-bind:productList="productList"
    />
  </div>
</template>

<script>
import PageWithProducts from "@/components/PageWithProducts";
export default {
  name: 'App',
  data() {
    return{
      productList: [
        {id: 1, title: 'Iphone', price: '10', shopURL: ''},
        {id: 2, title: 'Android', price: '100', shopURL: ''},
        {id: 3, title: 'Nokia', price: '20', shopURL: ''},
      ]
    }
  },
  components: {
    PageWithProducts
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
