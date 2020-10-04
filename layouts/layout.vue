<template>
  <v-app>
    <Header/>
    <v-container>
      <v-row justify="center" align="center">
        <v-col sm="12" md="8">
          <nuxt style="padding-top: 65px"></nuxt>
        </v-col>
      </v-row>
    </v-container>
    <Footer/>
  </v-app>
</template>

<script>
  import Header from '~/components/Header.vue'
  import Footer from '~/components/Footer.vue'

  export default {
    name: 'layout',
    components: {
      Header,
      Footer
    }
  }
</script>
