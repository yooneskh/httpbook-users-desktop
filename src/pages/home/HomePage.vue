<script setup>

import Sidebar from './sidebar/Sidebar.vue';

</script>

<template>
  <div class="page" fluid>

    <Sidebar class="sidebar" />

  </div>
</template>

<style lang="scss" scoped>
  .page {

    .sidebar {
      height: 100vh;
      width: 233px;
    }
  }
</style>
