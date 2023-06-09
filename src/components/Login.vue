<template>
  <v-container>
    <v-card>
      <v-card-title>Login</v-card-title>
      <v-card-text>
        <v-form @submit.prevent="login">
          <v-text-field v-model="username" label="Username"></v-text-field>
          <v-text-field
            v-model="password"
            label="Password"
            type="password"
          ></v-text-field>
          <v-btn type="submit">Login</v-btn>
        </v-form>
      </v-card-text>
    </v-card>
  </v-container>
</template>

<script setup>
//
</script>
