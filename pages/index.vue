<template>
  <v-container fluid>
    <v-row justify="center">
      <v-col
        cols="12"
        sm="12"
      >
        <v-card
          class="soku-card"
        >
          <v-card-title class="headline ma-3">
            <div class="soku">この男、即戦力・・・</div>
          </v-card-title>
          <v-spacer></v-spacer>
          <v-card-title class="ma-3">
            <div class="soku">即戦力な男。中野晃佑</div>
          </v-card-title>
        </v-card>
      </v-col>
      <v-col
        cols="12"
        sm="12"
        justify="center"
      >
        <img class="sokujpg" src="@/static/soku.JPG">
      </v-col>
    </v-row>
    <h3 style="text-align: center; color: black">inspired by 世界一即戦力な男・菊池良、あかしぃ</h3>
  </v-container>
</template>

<script>
  export default {
    layout: 'layout'
  }
</script>

<style>
  .sokujpg {
    height: 100%;
    width: 100%;
    border-radius: 10px;
  }

  .soku {
    font-weight: bold;
    font-size: 75px;
    margin: 10px
  }

  .soku-card {
    padding-top: 40px;
    height: 300px;
  }

  @media screen and (max-width: 768px) {
    .soku {
      font-weight: bold;
      font-size: 60px;
      margin: 0;
    }
  }

  @media screen and (max-width: 480px) {
    .sokujpg {
      width: 100%;
    }

    .soku {
      font-weight: bold;
      font-size: 20px;
      margin: 0;
    }

    .soku-card {
      height: 200px;
    }
  }
</style>
