<template>
  <v-container class="mt-4">
    <v-row class="justify-center">
      <v-col cols="6">
        <TheTopBar/>
        <PostList/>
      </v-col>

      <v-col cols="3">
        <TheSideBar style="border:1px solid red !important;"/>
      </v-col>

    </v-row>
  </v-container>
</template>

<script lang="ts">
import Vue from 'vue'
import PostList from "@/components/PostList.vue";
import TheSideBar from "@/components/TheSideBar.vue";
import TheTopBar from "@/components/TheTopBar.vue";

export default Vue.extend({
  name: 'Home',

  components: {
    TheTopBar,
    TheSideBar,
    PostList
  },
})
</script>
