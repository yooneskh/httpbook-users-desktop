<script setup>

import Sidebar from './sidebar/sidebar.vue';
import Tabbar from './tabbar/tabbar.vue';
import MainContent from './main-content/main-content.vue';
import MainResult from './main-result/main-result.vue';

</script>

<template>
  <div class="page" fluid>

    <sidebar class="sidebar" />

    <tabbar class="tabbar" />

    <main-content class="main-content" />

    <main-result class="main-result" />

  </div>
</template>

<style lang="scss" scoped>
  .page {

    height: 100vh;
    display: grid;

    grid-template-areas:
      '_S _T _R'
      '_S _M _R';

    grid-template-columns: 233px 1fr 380px;
    grid-template-rows: auto 1fr;

    .sidebar {
      grid-area: _S;
    }
    .tabbar {
      grid-area: _T;
    }
    .main-content {
      grid-area: _M;
    }
    .main-result {
      grid-area: _R;
    }
  }
</style>
