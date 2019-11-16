<template>
  <v-container>
    <v-row>
      <v-col cols="6">
        <img class="nandemojpg" src="@/static/nandemo.JPG">
      </v-col>
      <v-col cols="6">
        <v-card style="margin-bottom: 20px;">
          <v-card-text>
            <h1 style="margin: 20px;">経歴</h1>
            <ul style="margin: 30px;">
              <li style="margin: 10px 0;" v-for="history in histories" >
                {{ history }}
              </li>
            </ul>
          </v-card-text>
        </v-card>
        <v-card>
          <v-card-text>
            <h1 style="margin: 20px;">技術</h1>
            <ul style="margin: 30px;">
              <li style="margin: 10px 0;" v-for="technology in technologies" >
                {{ technology }}
              </li>
            </ul>
          </v-card-text>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    layout: 'layout',
    data() {
      return {
        histories: [
          "199412　熊本県出身",
          "201211　なんでも鑑定団に出演。出演者MVPを獲得",
          "201304　専修大学商学部マーケティング学科入学",
          "201405　取得単位数０で専修大学を中退。4年ほどフリーター活動に従事",
          "201811　SESの会社にて客先常駐社員として従事",
          "201907　株式会社コラビット入社 現在に至る"
        ],
        technologies: [
          "Rails(Ruby)",
          "Vue.js Nuxt.js",
          "Docker"
        ]
      }
    }
  }
</script>

<style>
  .nandemojpg {
    text-align: right;
    width: 400px;
  }
</style>
