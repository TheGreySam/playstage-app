<template>
  <v-carousel
    cycle
    height="400"
    hide-delimiter-background
    show-arrows-on-hover
  >
    <v-carousel-item
      v-for="(item, i) in items"
      :key="i"
      :src="item.src"
    >
   
      >
        <v-row
          class="fill-height"
          align="center"
          justify="center"
        >
         
        </v-row>
     
    </v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    data () {
      return {
          items: [
          {
            src: 'https://www.teatro-nescafe-delasartes.cl/wp-content/uploads/2022/03/mop_sebastian_dominguez_tna_19-1000x664.jpg',
          },
          {
            src: 'https://www.teatro-nescafe-delasartes.cl/wp-content/uploads/2022/03/mop_sebastian_dominguez_tna_17.jpg',
          },
          {
            src: 'https://www.teatro-nescafe-delasartes.cl/wp-content/uploads/2022/03/mop_sebastian_dominguez_tna_22.jpg',
          },
          {
            src: 'https://www.teatro-nescafe-delasartes.cl/wp-content/uploads/2022/03/mop_sebastian_dominguez_tna_24.jpg',
          },
        ],
       
     
      }
    },
  }
</script>