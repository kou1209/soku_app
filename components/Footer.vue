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
      <v-col cols="12" style="text-align: center; padding: 10px; 0">
        <a href="https://github.com/kou1209" target=”_blank”>
          <i class="fab fa-github fa-2x" style="color: black"></i>
        </a>
        <a href="https://twitter.com/knakano1209" target="_blank">
          <i class="fab fa-twitter fa-2x" style="color: #339af0;"></i>
        </a>
      </v-col>
      <v-col
        class="primary lighten-2 text-center white--text"
        xs="12"
        style="text-align: center; color: white; font-weight: bold"
      >
        {{ new Date().getFullYear() }} — Kosuke Nakano
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
            name: "Top",
            to: "/"
          },
          {
            name: "About",
            to: "/profile"
          },
          {
            name: "Works",
            to: "/works"
          },
          {
            name: "Contact",
            to: "/contact"
          }
        ]
      }
    }
  }
</script>
