<template>
  <v-container>
    <v-row class="text-center">
      <v-col
        class="mb-1"
        cols="12"
      >
        <h2 class="headline font-weight-bold mb-3">
          音楽検索
        </h2>
          <v-text-field
            v-model="keyword"
            :counter= "50"
            placeholder="アーティスト名を入れてね"
            required
          ></v-text-field>

          <v-btn @click="serch">検索</v-btn>
        <br>
      </v-col>
    </v-row>
    
  </v-container>
</template>

<script>
  export default {

    data: () => ({
      ecosystem: [

      ],
    })
  };
</script>
