<script setup>

import { reactive } from "vue";

const api = reactive({
  method: '',
  url: ''
});

</script>

<template>
  <div class="main-content pa-3 d-flex flex-row">

    <v-row dense>
      <v-col cols="1">
        <select class="y-select" v-model="api.method">
          <option>GET</option>
          <option>POST</option>
          <option>PUT</option>
          <option>PATCH</option>
        </select>
      </v-col>
      <v-col cols="10">
        <input type="text" class="y-input" v-model="api.url" />
      </v-col>
      <v-col cols="1">
        <button type="button" class="y-button">
          Run
        </button>
      </v-col>
    </v-row>

  </div>
</template>

<style lang="scss" scoped>
  .main-content {
    background-color: rgba(white, 0.0375);
  }
</style>