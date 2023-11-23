<template>
    <v-app>
      <v-navigation-drawer app v-model="drawer">
        <v-list>
          <v-list-item to="/user_management">
            <v-list-item-icon>
              <v-icon>mdi-account</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title>User Management</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item href="/user_manage">
            <v-list-item-icon>
              <v-icon>mdi-domain</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title>Branch Management</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item to="/inventory">
            <v-list-item-icon>
              <v-icon>mdi-archive</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
              <v-list-item-title>Inventory</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-navigation-drawer>
  
      <v-app-bar app color="primary">
        <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>
        <v-toolbar-title>Admin</v-toolbar-title>
        <v-spacer></v-spacer>
      </v-app-bar>
    </v-app>
  </template>
  
  <script>
  export default {
    data() {
      return {
        drawer: false,
      };
    },
  };
  </script>
  
  <style scoped>
  /* Add custom styles for the navbar if needed */
  </style>
  