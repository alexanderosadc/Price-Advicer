<template>
  <div>
    <ul>
      <product v-for="productItem of productList" :key="productItem.id" :product-item="productItem" />
    </ul>
  </div>

</template>

<script>

import Product from "@/components/Product";

export default {
  name: "PageWithProducts",
  props: ['productList'],
  components: {Product}
}
</script>

<style scoped>

</style>
