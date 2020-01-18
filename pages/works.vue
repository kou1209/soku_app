<template>
  <div>
    <v-row>
      <v-col cols="12" sm="12">
        <h1 style="font-family: Monaco">担当した業務</h1>
        <v-card style="margin-bottom: 20px;">
          <v-card-text>
            <h2 style="margin: 20px;">自社プロダクトの開発運用</h2>
            <p style="margin-bottom: 10px;">期間：2019年7月〜現在</p>
            <h3>RubyonRailsを用いた中〜大規模toC向けwebアプリの、新機能の開発、保守運用</h3>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
    <v-card style="margin-bottom: 20px;">
      <v-card-text>
        <h2 style="margin: 20px;">toB向けプロダクトの新機能開発</h2>
        <p style="margin-bottom: 10px;">期間：2019年9月〜2019年10月</p>
        <h3>Vue.jsを用いた既存のtoB向けSPAの新機能開発。<br>VueRouter、Vuexを使用し、単一ファイルコンポーネントを用いる形での実装を行いました。<br>UIコンポーネントにはVuetifyを利用しました。
        </h3>
      </v-card-text>
    </v-card>
    <v-card style="margin-bottom: 20px;">
      <v-card-text>
        <h2 style="margin: 20px;">toB向け新プロダクトの開発</h2>
        <p style="margin-bottom: 10px;">期間：2020年1月〜現在</p>
        <h3>RailsとNuxt.jsを用いたtoB向けSPAの新プロダクト開発。<br>APIにRails、フロントエンドにNuxt.jsを用いて現在進行形で開発を進めています。
        </h3>
      </v-card-text>
    </v-card>
  </div>
</template>
<script>
  export default {
    layout: 'layout'
  }
</script>
