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
      .col {
        padding-top: 40px;
        h3 {
          color: white;
          padding: 15px 20px;
        }
        ul {
          padding-left: 0;
          li {
            list-style: none;
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
}
</style>
