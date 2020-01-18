<template>
  <v-container fluid>
    <v-row justify="center">
      <v-col class="portfolio" cols="12">
        Nakano
        Portfolio
        Site
      </v-col>
      <img class="jpg" src="@/static/golden.JPG">
    </v-row>
  </v-container>
</template>

<script>
  export default {
    layout: 'layout'
  }
</script>

<style>
  .portfolio {
    font-size: 50px;
    font-style: oblique;
    margin-bottom: 20px;
  }

  .jpg {
    width: 100%;
    height: 100%;
  }
</style>
