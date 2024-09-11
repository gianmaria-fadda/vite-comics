<script>
export default {
  
}
</script>

<template>
  <div class="dc-items">
    <div>
      <img src="" :alt="Titolo">
    </div>

    <div>
      <p>
        Titolo
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
