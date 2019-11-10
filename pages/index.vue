<template>
  <v-container fluid>
    <v-row justify="center">
      <v-col
        cols="6"
        justify="center"
      >
        <img class="sokujpg" src="@/static/soku.JPG">
      </v-col>
      <v-col
        cols="6"
      >
        <v-card
          color="#385F73"
          dark
          style="height: 50%; padding-top: 40px"
        >
          <v-card-title class="headline ma-3" style="font-size: 50px">この男、即戦力・・・</v-card-title>
          <v-spacer></v-spacer>
          <v-card-subtitle class=ma-3 style="font-size: 50px">即戦力な男。中野晃佑</v-card-subtitle>
        </v-card>
      </v-col>
    </v-row>
    <h3 style="text-align: center; color: white">inspired by 世界一即戦力な男・菊池良、あかしぃ</h3>
  </v-container>
</template>

<script>
  export default {
    layout: 'layout'
  }
</script>

<style>
  .sokujpg {
    height: 700px;
    width: 100%;
    border-radius: 30px;
  }
</style>
