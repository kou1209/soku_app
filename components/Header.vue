<template>
  <v-card class="overflow-hidden" style="position: relative">
    <v-app-bar
      color="#6A76AB"
      dark
      shrink-on-scroll
      prominent
      src="https://picsum.photos/1920/1080?random"
      fade-img-on-scroll
      scroll-target="#scrolling-techniques-3"
    >
      <template v-slot:img="{ props }">
        <v-img
          v-bind="props"
          gradient="to top right, rgba(100,115,201,.7), rgba(25,32,72,.7)"
        ></v-img>
      </template>
      <v-spacer></v-spacer>
      <v-toolbar-title>即戦力</v-toolbar-title>
      <v-spacer></v-spacer>
      <template v-slot:extension>
        <v-tabs
          background-color="transparent"
        >
          <v-spacer></v-spacer>
          <v-tab v-for="(link, index) in links" :key="index">
            <nuxt-link style="color: white; text-decoration: none" :to="link.to">
              {{link.name}}
            </nuxt-link>
          </v-tab>
          <v-spacer></v-spacer>
        </v-tabs>
      </template>
    </v-app-bar>
    <v-sheet
      id="scrolling-techniques-3"
      class="overflow-y-auto"
      max-height="600"
    >
    </v-sheet>
  </v-card>
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
