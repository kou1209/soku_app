<template>
  <div style="background-color: #EEEEEE;">
    <Header/>
    <v-container>
      <v-row>
        <v-col xs="12">
          <nuxt style="padding-top: 60px"></nuxt>
        </v-col>
      </v-row>
    </v-container>
    <Footer/>
  </div>
</template>

<script>
  // ヘッダ＆フッタをインポート
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
