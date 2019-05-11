<template>
  <div class="promo-page">
    <div class="promo-block1">
      <v-container>
        <v-layout align-center justify-space-between column fill-height>
          <v-img class="promo-logo" src="/img/Logo.jpg" width="50vh" max-width="100%"></v-img>
          <span class="promo-title">Burner Game Studio</span>
          <span class="promo-subtitle">Мы что то пилим...</span>
        </v-layout>
      </v-container>
    </div>
    <div class="promo-block2">
      <v-img src="/img/Arts/ComboImage.png" min-height="90vh">
        <div class="promo-block2-left">
          <h1>Тут что то должно быть что то пафосное с ссылочками и иконочками 1...</h1>
        </div>
        <div class="promo-block2-right">
          <h1>Тут что то должно быть что то пафосное с ссылочками и иконочками 2...</h1>
        </div>
      </v-img>
    </div>
    <div class="promo-block3">
      <v-container>
        <v-layout column align-center justify-center fill-height>
          <v-img src="/img/FohLogo.png" width="70vw"></v-img>
          <div>
            <h1>Что то про Field of Honor...</h1>
          </div>
        </v-layout>
      </v-container>
    </div>
    <div class="promo-block4">
      <v-container>
        <v-layout align-center justify-center row>
          <h1>Контакты</h1>
        </v-layout>
        <v-layout row align-center justify-center fill-height>
          <div>&nbsp;</div>
        </v-layout>
        <v-layout row align-center justify-center fill-height>
          <v-flex xs1 mr-5><v-img class="social-image" src="/img/socials/twitter.png"></v-img></v-flex>
          <v-flex xs1 mr-5><v-img class="social-image" src="/img/socials/facebook.png"></v-img></v-flex>
          <v-flex xs1 mr-5><v-img class="social-image" src="/img/socials/vk.png"></v-img></v-flex>
          <v-flex xs1 mr-5><v-img class="social-image" src="/img/socials/instagram.png"></v-img></v-flex>
          <v-flex xs1><v-img class="social-image" src="/img/socials/gmail.png"></v-img></v-flex>
        </v-layout>
        <v-layout row align-center justify-center fill-height hidden-sm-and-down>
          <v-flex xs1 mr-5 class="text-xs-center">Twitter</v-flex>
          <v-flex xs1 mr-5 class="text-xs-center">Facebook</v-flex>
          <v-flex xs1 mr-5 class="text-xs-center">Vkontakte</v-flex>
          <v-flex xs1 mr-5 class="text-xs-center">Instagram</v-flex>
          <v-flex xs1 class="text-xs-center">Gmail</v-flex>
        </v-layout>
      </v-container>
    </div>
    <div class="promo-block5">
      <v-container>
        <v-layout column align-center justify-center fill-height>
          <v-flex xs2><h1>Поддержи нас</h1></v-flex>
          <v-flex xs2>Тут будут патреон, кошельки и прочее...</v-flex>
        </v-layout>
      </v-container>
    </div>
  </div>
</template>

<script>
  export default {
    data: () => ({
    })
  }
</script>

<style lang="stylus">
  @import '../assets/style/utilities.styl';

  .promo-page {
    .promo-block {
      &1 {
        min-height: 90vh;
        background: radial-gradient(#506b74, #2b2b2b);
      }
      &2 {
        &-left {
          position: absolute;
          left: 10vw;
          bottom: 15vh;
          max-width: 30vw;
        }

        &-right {
          position: absolute;
          right: 15vw;
          top: 15vh;
          max-width: 30vw;
        }
      }
      &3 {
        background: url('/img/Arts/Dragon_fire.jpg');
      }
      &4 {
        background-color: #495c63;
        font-size: 20px;
      }
    }

    .social-image {
      transition .2s;

      &:hover {
        transform scale(1.1);
      }
    }

    .v-image__image {
      background-position: center top !important;
    }

    .promo-logo {

    }

    .promo-title {
      font-size: 8vh;
      font-weight: bold;
      color: #dddddd;
    }

    .promo-subtitle {
      font-size: 3vh;
      font-weight: bold;
      color: #aaaaaa;
    }
  }
</style>