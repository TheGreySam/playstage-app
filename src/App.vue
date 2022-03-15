<template>
  <v-app>
    <v-app-bar app color="rgb(0, 142, 185)" dark>
      <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
      <v-img 
      img 
      contain 
      max-height="50"
 
  alt="Vue logo" src="./assets/ps logo-lite.png"></v-img>

      <v-toolbar-title>Playstage App</v-toolbar-title>
      <v-spacer></v-spacer>
      
    </v-app-bar>
    <v-navigation-drawer v-model="drawer" fixed expand-on-hover permanent>
    
      <v-list nav dense>
        <v-list-item-group v-model="group" active-class=" text--accent-4">
          
            <v-img
              img
              alt="Vue logo"
              src="./assets/PSisotipo-lite.svg"
              max-width="150"
            ></v-img>
          
          <v-list-item to="/">
            <v-list-item-icon>
              <v-icon>mdi-home</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item>

          <v-list-item to="/login">
            <v-list-item-icon>
              <v-icon>mdi-account</v-icon>
            </v-list-item-icon>
            <v-list-item-title>Login</v-list-item-title>
          </v-list-item>

        </v-list-item-group>
      </v-list>
    </v-navigation-drawer>

    <v-main>
      <v-parallax dark height="500" src="./assets/White_BG.jpg">
        <router-view fluid/>
      </v-parallax>

      
    </v-main>

    <Footer />
  </v-app>
</template>

<script>
export default {
  name: "App",
  components: {
    //Navbar: () => import("./components/Navbar"),
    Footer: () => import("./components/Footer.vue"),

  },

  data: () => ({
    drawer: false,
    group: null,
  }),
};
</script>
