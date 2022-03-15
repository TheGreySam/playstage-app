<template>
  <v-footer dark padless>
    <v-card class="flex" flat tile>
      <v-card-text class="footer white--text text-center">
        <strong>Biznet It Tecnologias de Informacion</strong>
      </v-card-text>

      <v-card-text class="py-2 white--text text-center">
        <strong>Playstage App</strong> - {{ new Date().getFullYear() }}
      </v-card-text>
    </v-card>
  </v-footer>
</template>


<style>
.footer {
  padding: 15px;
  background-color: rgb(0, 142, 185);
}
</style>
