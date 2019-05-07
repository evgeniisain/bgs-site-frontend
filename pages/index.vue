<template>
  <div class="promo-page">
    <div class="promo-block1">
      <v-container>
        <v-layout row wrap justify-center align-center>
          <v-flex xs3>
            <v-img class="promo-logo" src="/img/Logo.jpg" width="300px"></v-img>
          </v-flex>
        </v-layout>
        <v-layout row wrap justify-center align-center>
          <v-flex xs5>
            <span class="promo-title">Burner Game Studio</span>
          </v-flex>
        </v-layout>
      </v-container>
    </div>
    <div class="promo-block2">
      <v-container>

      </v-container>
    </div>
  </div>
</template>

<script>
  import { PromoContentType } from '../constants/promo-content-type'

  export default {
    data: () => ({
      carouselItems: [
        {
          content: '',
          type: PromoContentType.image,
          url: '/img/Art.jpg'
        }
      ]
    })
  }
</script>

<style lang="stylus">
  .promo-page {
    .promo-block1 {
      min-height 80vh;
      background: radial-gradient(#506b74, #2b2b2b);
    }

    .v-image__image {
      background-position center top !important;
    }

    .promo-logo {

    }

    .promo-title {
      font-size 8vh;
      font-weight bold;
      color #dddddd;
    }
  }
</style>