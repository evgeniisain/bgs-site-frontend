<template>
  <v-app dark>
    <v-toolbar scroll-off-screen app>
      <v-toolbar-title v-text="title"></v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn
        v-for="(item, index) in items"
        :key="index"
        :to="item.to"
        icon
      >
        <v-icon>{{item.icon}}</v-icon>
      </v-btn>
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
        items: [
          {
            icon: 'apps',
            title: 'Welcome',
            to: '/'
          },
          {
            icon: 'bubble_chart',
            title: 'Inspire',
            to: '/inspire'
          }
        ],
        title: 'Burner Game Studio'
      }
    }
  }
</script>
