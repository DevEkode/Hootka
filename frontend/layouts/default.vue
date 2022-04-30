<template>
  <v-app>
    <v-app-bar app>
      
      <v-img 
        class="logo d-flex ml-auto" 
        lazy-src="logo.svg" 
        src="logo.svg"
        max-height="50"
        max-width="200"
        contain>
      </v-img>
      <v-spacer></v-spacer>

      <!-- Account login / register -->
      <v-menu offset-y>
        <template v-slot:activator="{ on, attrs }">
          <v-btn flat icon color="primary" dark v-bind="attrs" v-on="on">
            <v-icon>mdi-account-circle</v-icon>
          </v-btn>
        </template>
        <v-list>
          <v-list-item-group>
            <v-list-item v-for="(item, index) in AccountItems" :key="index" :to="item.href">
              <v-list-item-icon>
                <v-icon>{{ item.icon }}</v-icon>
              </v-list-item-icon>
              <v-list-tile-content>
                <v-list-item-title>{{ item.text }}</v-list-item-title>
              </v-list-tile-content>
            </v-list-item>
          </v-list-item-group>
        </v-list>
      </v-menu>
    </v-app-bar>

    <!-- Sizes your content based upon application components -->
    <v-main>
      <v-container fluid>
        <Nuxt />
      </v-container>
    </v-main>

    <v-footer app>
      <!-- -->
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: "DefaultLayout",
  data() {
    return {
      AccountItems: [
        { text: "Login", icon: "mdi-login", href: "/login" },
        { text: "Register", icon: "mdi-account-plus", href: "/register" },
      ],
    };
  },
};
</script>

<style>
  .logo {
    filter: brightness(0) invert(1);
  }
</style>
