<template>
  <div class="md-layout">
    <div class="md-layout-item md-medium-size-33 md-small-size-30 md-xsmall-size-100">
      <md-card>
        <md-card-header>
          <md-card-header-text>
            <div class="md-title">{{productItem.title}}</div>
          </md-card-header-text>
        </md-card-header>
        <md-card-content>
          <md-card-media>
<!--            <img :src="image" height="250" alt="{{productItem.title}}}">-->
          </md-card-media>
          <span>
            <a :href =productItem.url>{{productItem.price}}</a>
          </span>
        </md-card-content>
      </md-card>
    </div>
  </div>
</template>

<script>
export default {
  name: "Product",
  props: {
    productItem:{
      type:Object,
      required: true
    }
  }
}
</script>

<style scoped>

</style>
