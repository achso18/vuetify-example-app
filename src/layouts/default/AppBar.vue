<template>
  <v-app-bar :elevation="10">
    <v-app-bar-title>
      {{ appTitle }}
    </v-app-bar-title>
    <v-toolbar-items class="hidden-xs-only">
      <v-btn flat v-for="item in menuItems" :key="item.title" :to="item.path">
        <v-icon left dark>{{ item.icon }}</v-icon>
        {{ item.title }}
      </v-btn>
    </v-toolbar-items>
    <v-spacer></v-spacer>
    <v-btn icon="mdi-login" :key="'login'" :to="'/login'"></v-btn>
  </v-app-bar>
</template>

<script setup>
const sidebar = false;
const menuItems = [{ title: "Home", icon: "mdi-home", path: "/" }];
const appTitle = "My App";
</script>
