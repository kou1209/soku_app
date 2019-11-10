<template>
  <div style="background: #212121;">
    <Header/>
    <nuxt style="width: 80%"></nuxt>
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
