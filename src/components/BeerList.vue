<template>
  <v-container fluid>
    <beer-card></beer-card>
  </v-container>
</template>

<script>
import BeerCard from '@/components/BeerCard.vue'

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

  },
  method:{
      
  }
}
</script>

<style>
</style>