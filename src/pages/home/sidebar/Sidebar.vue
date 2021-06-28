<script setup>

import SidebarProjectSelector from "./components/SidebarProjectSelector.vue";
import SidebarItemsToolbar from "./components/SidebarItemsToolbar.vue";
import SidebarItems from "./components/SidebarItems.vue";

</script>

<template>
  <div class="sidebar">

    <SidebarProjectSelector class="project-selector" />

    <SidebarItemsToolbar class="items-toolbar" />

    <SidebarItems class="items" />

  </div>
</template>

<style lang="scss" scoped>
  .sidebar {
    border-right: 1px solid rgba(white, 0.15);
    display: flex;
    flex-direction: column;
    & > .project-selector {
      flex-grow: 0;
      flex-shrink: 0;
    }
    & > .items-toolbar {
      flex-grow: 0;
      flex-shrink: 0;
    }
    & > .items {
      height: 0;
      flex-grow: 1;
      overflow-y: auto;
    }
  }
</style>