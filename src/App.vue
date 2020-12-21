<template>
  <div id="app">
    <v-app>
      <navbar></navbar>
      <!-- Sizes your content based upon application components -->
      <v-main>
        <!-- Provides the application the proper gutter -->
        <v-container fluid>
          <!-- If using vue-router -->
          <router-view></router-view>
        </v-container>
      </v-main>

      <v-footer app>
        <!-- -->
      </v-footer>
    </v-app>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue';

export default{
  name:'App',
  components: {
        Navbar
    }
}
</script>

<style lang="scss">
</style>
