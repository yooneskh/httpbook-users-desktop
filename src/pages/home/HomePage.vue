<script setup>

import Sidebar from './sidebar/Sidebar.vue';
import Tabbar from './tabbar/Tabbar.vue';
import MainContent from './main-content/MainContent.vue';

</script>

<template>
  <div class="page" fluid>

    <Sidebar class="sidebar" />

    <Tabbar class="tabbar" />

    <MainContent class="main-content" />

  </div>
</template>

<style lang="scss" scoped>
  .page {
    height: 100vh;
    display: grid;

    grid-template-areas:
      '_S _T'
      '_S _M';

    grid-template-columns: 233px auto;
    grid-template-rows: 36px auto;

    .sidebar {
      grid-area: _S;
    }
    .tabbar {
      grid-area: _T;
    }
    .main-content {
      grid-area: _M;
    }
  }
</style>
