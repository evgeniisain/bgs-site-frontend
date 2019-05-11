<template>
  <v-app dark>
    <v-toolbar scroll-off-screen app>
      <v-toolbar-title v-text="title"></v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn><v-icon>info</v-icon>&nbsp;Новости</v-btn>
      <v-btn><v-icon>question_answer</v-icon>&nbsp;ЧАВО</v-btn>
      <v-btn><v-icon>people</v-icon>&nbsp;Сообщество</v-btn>
      <v-btn><v-icon>build</v-icon>&nbsp;Проекты</v-btn>
      <v-btn><v-icon>image</v-icon>&nbsp;Галлерея</v-btn>
      <v-btn><v-icon>help</v-icon>&nbsp;О нас</v-btn>
    </v-toolbar>
    <v-content>
      <nuxt />
    </v-content>
    <v-footer class="justify-center" absolute app>
      <Footer />
    </v-footer>
  </v-app>
</template>

<script>
  import Footer from '../components/Footer'

  export default {
    components: { Footer },
    data () {
      return {
        title: 'Burner Game Studio'
      }
    }
  }
</script>
