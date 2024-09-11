<script>
export default {
  props: {
    product: Object
  }
}
</script>

<template>
  <div class="dc-items">
    <div>
      <img :src="product.thumb" :alt="product.series">
    </div>

    <div>
      <p>
        {{ product.series }}
      </p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.dc-items {
  
  > * {
    padding: 10px 190px;
    width: 25%;

    p {
      color: white;
      text-align: center;
      padding: 4px;
    }
  }
}
</style>
