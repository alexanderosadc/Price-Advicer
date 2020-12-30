<template>
  <div class="md-layout">
      <product class="md-layout-item md-gutter md-medium-size-33 md-small-size-50 md-xsmall-size-100"
               v-for="productItem of productList" :key="productItem.id" :product-item="productItem"
      />
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

<style lang="scss" scoped>

</style>
