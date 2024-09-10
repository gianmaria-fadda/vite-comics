<script>
export default {
  data() {
    return{
      images:[
        'img/buy-comics-digital-comics.png',
        'img/buy-comics-merchsndise.png',
        'img/buy-comics-shop-locator.png',
        'img/buy-comics-subscriptions.png',
        'img/buy-dc-power-visa.svg.png'
      ]
    }
  }
}
</script>

<template>
<main>
    <div class="container">
      <a href="#">&rarr; Content click here &larr;</a>
    </div>
    <div class="container">
      <div>
        <img src="../assets/img/buy-comics-digital-comics.png" alt="foto">

        <p>
          DIGITAL COMICS
        </p>
      </div>

      <div>
        <img src="../assets/img/buy-comics-merchandise.png" alt="foto">

        <p>
          DC MERCHANDISE
        </p>
      </div>

      <div>
        <img src="../assets/img/buy-comics-shop-locator.png" alt="foto">

        <p>
          SUBSCRIPTION
        </p>
      </div>

      <div>
        <img src="../assets/img/buy-comics-subscriptions.png" alt="foto">

        <p>
          COMICS SHOP LOCATOR
        </p>
      </div>

      <div>
        <img src="../assets/img/buy-dc-power-visa.svg" alt="foto">

        <p>
          DC POWER VISA
        </p>
      </div>
    </div>
  </main>
</template>

<style scoped>
main {
  background-color: #1C1C1C;
  .container {
    padding: 50px 0;
    a {
      text-decoration: none;
      color: white;
      font-size: 2.5cap;
      padding-left: 230px;
    }
  }
  .container:last-child {
    display: flex;
    justify-content: space-evenly;
    background-color: #0282F9;
    padding: 50px 200px;
    div {
      display: flex;
      align-items: center;
      img {
        width: 50px;
        object-fit: contain;
      }
      p {
        color: white;
        padding: 0 10px;
      }
      &:hover {
          cursor: pointer;
      }
    }
  }
}
</style>
