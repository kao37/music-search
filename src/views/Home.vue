<template>
  <v-container>
<v-parallax xs12 sm6 md4
    height="300" 
    src="https://images.pexels.com/photos/1105666/pexels-photo-1105666.jpeg?auto=compress&cs=tinysrgb&h=650&w=940"></v-parallax>
<!-- https://www.u4get.com/wp-content/uploads/2019/02/TE-D01d_model-1140x641.jpg -->

<!-- https://i.ytimg.com/vi/vsFi9jPnQ9E/maxresdefault.jpg -->
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
            <v-btn rounded color="pink darken-1" dark @click="search">-検索-</v-btn>
        </v-col>
    </v-row>
  </v-container>
</template>
<script>
export default {
  data(){
    return{
      keywprd: '',
    }
  },
  methods:{
    search(){
      this.$router.push(`/result/${this.keyword}`)
    }
  }
};
</script>
