<template>
  <v-tabs
    fixed-tabs
    background-color="indigo"
    dark
    class="tabs"
  >
    <v-tab v-for="(link, index) in links" :key="index"
           style="color: white; text-decoration: none" :to="link.to">
      {{link.name}}
    </v-tab>
  </v-tabs>
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

<style>
  .tabs {
    text-align: center;
  }
</style>
