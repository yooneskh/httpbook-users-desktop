<script setup>

import TabItem from "./components/tab-item.vue";

const activeTab = ref(3);

</script>

<template>
  <div class="tabbar">

    <tab-item
      v-for="tab of 9" :key="tab"
      class="tab-item"
      :active="tab === activeTab"
      @click="activeTab = tab"
      @close="activeTab = -1"
    />

  </div>
</template>

<style lang="scss" scoped>
  .tabbar {
    border-bottom: 1px solid rgba(white, 0.075);
    white-space: nowrap;
    .tab-item {
      display: inline-block;
    }
  }
</style>