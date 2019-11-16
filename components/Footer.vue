<template>
  <v-footer
    color="#424242"
    padless
    height="160px;"
  >
    <link href="https://use.fontawesome.com/releases/v5.0.13/css/all.css" rel="stylesheet">
    <v-row
      no-gutters
      justify="center"
    >
      <v-col xs="12">
        <div style="text-align: center">
          <v-btn
            v-for="(link, index) in links"
            :key="index"
            style="color: white;"
            text
            rounded
            class="my-2"
            :to="link.to"
          >
            {{ link.name }}
          </v-btn>
        </div>
      </v-col>
      <v-col cols="12">
        <div style="text-align: center; margin-top: 20px;">
          <i class="fab fa-github fa-3x"></i>
          <i style="color: #339af0;" class="fab fa-twitter fa-3x"></i>
        </div>
      </v-col>
      <v-col
        class="primary lighten-2 py-4 text-center white--text"
        xs="12"
      >
        <div style="text-align: center; color: white; margin-top: 20px">
          {{ new Date().getFullYear() }} — <strong>即戦力な男。中野晃佑</strong>
        </div>
      </v-col>
    </v-row>
  </v-footer>
</template>

<script>
  export default {
    data() {
      return {
        links: [
          {
            name: "即戦力な男とは・・・",
            to: "/"
          },
          {
            name: "即戦力な経歴",
            to: "/profile"
          },
          {
            name: "担当した業務",
            to: "/works"
          },
          {
            name: "連絡する",
            to: "/contact"
          }
        ]
      }
    }
  }
</script>
