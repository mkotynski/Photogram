<template>
  <v-app>
    <v-app-bar
        app
        color="white"
        style="border-bottom:1px solid #e2e2e2 !important;"
        elevation="0"
        height="50"
    >
      <div class="d-flex ml-2">
        <span style="color:#414141">
          {{ title }}
        </span>
      </div>

      <v-spacer></v-spacer>
    </v-app-bar>

    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
  name: 'App',
  data: () => ({
    title: 'PHOTOGRAM',
  }),
});
</script>

<style>
#app {
  margin: 0;
  padding: 0;
  background-color: #fafafa;
}

.outline-border {
  border: 1px solid #dbdbdb !important;
  border-radius: 3px !important;
  background-color:white !important;
}
</style>
