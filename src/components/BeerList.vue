<template>
  <v-container fluid>
    <beer-card v-for="beer of beers" :key="beer.id" :beer="beer"></beer-card>
  </v-container>
</template>

<script>
import BeerCard from '@/components/BeerCard.vue'
import axios from 'axios'

export default {
 name: 'BeerList',
  components: {
    BeerCard
  },
  
  data(){
      return {
      beers:[],
      };
  },
  mounted(){
      axios.get('https://api.punkapi.com/v2/beers').then(
          (response)=>{
              this.beers = response.data;
          }
      ).catch(error=>{
          console.log(error);
      })
  },
  method:{

  }
}
</script>

<style>
</style>