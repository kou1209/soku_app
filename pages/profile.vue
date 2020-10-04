<template>
  <v-container>
    <v-row>
      <v-col cols="12" >
        <img class="nandemojpg" src="@/static/nandemo.JPG">
      </v-col>
      <v-col cols="12" >
        <v-card class="mb-5">
          <v-card-text>
            <h1 style="margin: 20px;">経歴</h1>
            <ul style="margin: 30px;">
              <li style="margin: 10px 0;" v-for="history in histories">
                {{ history }}
              </li>
            </ul>
          </v-card-text>
        </v-card>
        <v-card class="mb-5">
          <v-card-text>
            <h1 style="margin: 20px;">技術</h1>
            <ul style="margin: 30px;">
              <li style="margin: 10px 0;" v-for="technology in technologies">
                {{ technology }}
              </li>
            </ul>
          </v-card-text>
        </v-card>
        <v-card>
          <v-card-text>
            <h1 style="margin: 20px;">条件</h1>
            <ul style="margin: 30px;">
              <li style="margin: 10px 0;">
                以前の副業ではNuxtで3000（税別）で稼働していたので、vueもしくはNuxtだと4000（税別）で稼働したいと考えております。<br>
                Reactの場合は経験が少ないので3000（税別）で稼働したいと考えております。
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
          "1994/12　熊本県出身",
          "2012/11　なんでも鑑定団に出演。出演者MVPを獲得",
          "2013/04　専修大学商学部マーケティング学科入学",
          "2014/05　取得単位数０で専修大学を中退。4年ほどフリーター活動に従事",
          "2018/11　SESの会社にて客先常駐社員として従事",
          "2019/07　株式会社コラビット入社 現在に至る"
        ],
        technologies: [
          "Ruby / Ruby On Rails",
          "JavaScript",
          "TypeScript（少し）",
          "Vue.js / Nuxt.js",
          "Docker",
          "React（少し）",
          "Firebase（少し）",
          "AWS（少し）"
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

  @media screen and (max-width: 480px) {
    .nandemojpg {
      width: 100%;
    }
  }
</style>
