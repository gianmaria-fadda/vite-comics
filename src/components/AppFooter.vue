<script>
export default {
  data() {
    return{
      linkFirst: [
        'Character',
        'Comics',
        'Movies',
        'TV',
        'Games',
        'Videos',
        'News'
      ],
      linkSecond: [
        'Shop DC',
        'Shop DC Collectibles'
      ],
      linkThird: [
        'Term of Use',
        'Privacy Policy (New)',
        'Ad Choise',
        'Adversting',
        'Jobs',
        'Subscription',
        'Talent Workshop',
        'CPSC Certificates',
        'Ratings',
        'Shop Help',
        'Contact Us'
      ],
      linkFourth: [
        'DC',
        'MAD Magazine',
        'DC Kids',
        'DC Univerce',
        'DC Power Visa'
      ]
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
            <li v-for="(link, i) in linkFirst">
              {{ link }}
            </li>
          </ul>
          <h3>
            SHOP
          </h3>
          <ul>
            <li v-for="(link, i) in linkSecond">
              {{ link }}
            </li>
          </ul>
        </div>
        <div class="col">
          <h3>
            DC
          </h3>
          <ul>
            <li v-for="(link, i) in linkThird">
              {{ link }}
            </li>
          </ul>
        </div>
        <div class="col">
          <h3>
            SITES
          </h3>
          <ul>
            <li v-for="(link, i) in linkFourth">
              {{ link }}
            </li>
          </ul>
        </div>
      </div>
      <div class="row">
        <img src="../assets/img/dc-logo-bg.png" alt="dc-logo-bg">
      </div>
    </div>
    <div class="container">
      <div>
        <p>

          SIGN UP NOW!
          
        </p>
      </div>
      <div>
        <p>
          FOLLOW US
        </p>

        <img src="../assets/img/footer-facebook.png" alt="facebook">

        <img src="../assets/img/footer-periscope.png" alt="periscope">

        <img src="../assets/img/footer-pinterest.png" alt="pinterest">

        <img src="../assets/img/footer-twitter.png" alt="twitter">

        <img src="../assets/img/footer-youtube.png" alt="youtube">
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>

@mixin flex-rule {
  display: flex;
}

@mixin flex-rule-and-around {
  display: flex;
  justify-content: space-around;
}

@mixin list-none {
  list-style: none;
}

footer {

  .container:first-child {
    background-image: url(../assets/img/footer-bg.jpg);
    @include flex-rule-and-around;

    .list {
      @include flex-rule;

      .col {
        padding-top: 40px;

        h3 {
          color: white;
          padding: 15px 20px;
        }

        ul {
          padding-left: 0;

          li {
            @include list-none;
            padding: 1px 20px;
            color: #818181;
            font-size: .8rem;
          }
        }
      }
    }

    .row {
      img {
        width: 350px;
        object-fit: contain;
      }
    }
  }
  .container:last-child {
    @include flex-rule-and-around;
    align-items: center;
    max-height: 100vh;
    background-color: #303030;

    div:first-child {
      margin: 45px 0;

      p {
        font-weight: bold;
        padding: 15px;
        border: 1px solid #0282F9;
        color: white;
      }
    }

    div:last-child {
      @include flex-rule;
      align-items: center;

      p {
        font-weight: bold;
        color: #0282F9;
        padding: 0 10px;
      }

      img {
        width: 35px;
        margin: 0 10px;
      }
    }
  }
}
</style>
