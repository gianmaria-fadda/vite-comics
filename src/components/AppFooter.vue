<script>
export default {
  data() {
    return{
      
    }
  }
}
</script>

<template>
  <footer>
    <div class="container">
      <div class="row list">
        <div class="col">
        <h3>
          DC COMICS
        </h3>
        <ul>
          <li>
            
          </li>
        </ul>
        <h3>
          SHOP
        </h3>
      </div>
      <div class="col">
        <h3>
          DC
        </h3>
      </div>
      <div class="col">
        <h3>
          SITES
        </h3>
      </div>
      </div>
      <div class="row">
        <img src="../assets/img/dc-logo-bg.png" alt="dc-logo-bg">
      </div>
    </div>
    <div class="container">
      
    </div>
  </footer>
</template>

<style scoped>
footer {
  .container:first-child {
    background-image: url(../assets/img/footer-bg.jpg);
    display: flex;
    justify-content: space-around;
    .list {
      display: flex;
    }
    .row {
      img {
        width: 350px;
        object-fit: contain;
      }
    }
  }
}
</style>
