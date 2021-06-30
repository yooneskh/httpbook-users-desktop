<script setup>

import { ref } from "vue";
import TabItem from "./components/TabItem.vue";

const activeTab = ref(3);

</script>

<template>
  <div class="tabbar">

    <TabItem
      v-for="tab of 12" :key="tab"
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