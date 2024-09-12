<script>
export default {
  data() {
    return{
      link: [
        'CHARACTER',
        'COMICS',
        'MOVIES',
        'TV',
        'GAMES',
        'COLLECTIBLES',
        'VIDEOS',
        'FANS',
        'NEWS',
        'SHOP',
      ]
    }
  }
}
</script>

<template>
  <header>
    <div class="container">
      <img src="../assets/img/dc-logo.png" alt="img">
  
      <ul>
        <li v-for="(link, index) in link">
          {{ link }}
        </li>
      </ul>
    </div>
  </header>
</template>

<style lang="scss" scoped>

@use '../assets/scss/partials/mixins.scss' as *;

header {
  .container {
    @include flex-rule-and-around;
    img {
      width: 80px;
      padding: 20px 0;
      object-fit: contain;
    }
    ul {
      @include list-none;
      @include flex-rule;
      align-items: center;
      li {
        padding: 0 15px;
        font-weight: bold;
        opacity: .7;
      }
    }
  }
}
</style>
