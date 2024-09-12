<script>
import SingleComics from './SingleComics.vue';

export default {
  data() {
    return{
      images: [
        'img/buy-comics-digital-comics.png',
        'img/buy-comics-merchsndise.png',
        'img/buy-comics-shop-locator.png',
        'img/buy-comics-subscriptions.png',
        'img/buy-dc-power-visa.svg.png'
      ],
      comics: [
      {
          "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
          "price": "$19.99",
          "series": "Action Comics",
          "type": "comic book",
      },
      {
          "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
          "price": "$3.99",
          "series": "American Vampire 1976",
          "type": "comic book",
      },
      {
          "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
          "price": "$16.99",
          "series": "Aquaman",
          "type": "graphic novel",
      },
      {
          "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
          "price": "$2.99",
          "series": "Batgirl",
          "type": "comic book",
      },
      {
          "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
          "price": "$3.99",
          "series": "Batman",
          "type": "comic book",
      },
      {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
          "price": "$2.99",
          "series": "Batman Beyond",
          "type": "comic book",
      },
      {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
          "price": "$3.99",
          "series": "Batman/Superman",
          "type": "comic book",
      },
      {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
          "price": "$4.99",
          "series": "Batman/Superman Annual",
          "type": "comic book",
      },
      {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
          "price": "$5.99",
          "series": "Batman: The Joker War Zone",
          "type": "comic book",
      },
      {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
          "price": "$6.99",
          "series": "Batman: Three Jokers",
          "type": "comic book",
      },
      {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
          "price": "$4.99",
          "series": "Batman: White Knight Presents: Harley Quinn",
          "type": "comic book",
      },
      {
          "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
          "price": "$16.99",
          "series": "Catwoman",
          "type": "graphic novel",
      },
      ]
    };
  },
  components: {
    SingleComics
  }
};
</script>

<template>
<main>
    <div class="container">
      <h1>

        CURRENT SERIES 

      </h1>

      <div class="dc-container">
        <SingleComics
          v-for="(comics, i) in comics"
          :key="i"
          :product="comics"/>
      </div>
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

<style lang="scss" scoped>

@use '../assets/scss/partials/mixins.scss' as *;

main {
  background-color: #1C1C1C;
  
  .container {
    padding: 50px 0;

    h1 {
      text-align: center;
      width: 200px;
      @include white-color-rule;
      font-size: 1rem;
      margin-left: 170px;
      padding: 20px;
      @include blue-color-rule;
      margin-bottom: 20px;
    }

    .dc-container {
      @include flex-rule;
      justify-content: center;
      flex-wrap: wrap;

      > * {
        padding: 10px 190px;
        width: 25%;

        p {
          @include white-color-rule;
          text-align: center;
          padding: 4px;
        }
      }
    }
  }

  .container:last-child {
    @include flex-rule;
    justify-content: space-evenly;
    @include blue-color-rule;
    padding: 50px 200px;

    div {
      @include flex-rule;
      align-items: center;

      img {
        width: 50px;
        object-fit: contain;
      }

      p {
        @include white-color-rule;
        padding: 0 10px;
      }

      &:hover {
          cursor: pointer;
      }
    }
  }
}
</style>
