<template>
  <v-row fluid class="home" align="center" justify="center">
    <v-col class="text-center" cols="12">
      <Carousel/>
      <h1 class="text-h4 font-weight-thin mb-4" color="green">Playstage App</h1>
      <v-container>
        <h4 class="subheading">
          Una aplicacion para teatros
        </h4>
      </v-container>
      <v-spacer></v-spacer>
     
    </v-col>
    
  </v-row>
</template>

<script>

export default {
  name: "Home",
  components: { 
   Carousel: () => import("../components/Carousel.vue"),
   },
};
</script>

<style scoped>
.home {
  color: rgb(0, 142, 185);
  
}
</style>
