<script setup>

import SidebarProjectSelector from "./components/sidebar-project-selector.vue";
import SidebarItemsToolbar from "./components/sidebar-items-toolbar.vue";
import SidebarItems from "./components/sidebar-items.vue";

</script>

<template>
  <div class="sidebar">

    <sidebar-project-selector class="project-selector" />

    <sidebar-items-toolbar class="items-toolbar" />

    <sidebar-items class="items" />

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