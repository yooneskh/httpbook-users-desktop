<script setup>

import SidebarItem from "./sidebar-item.vue";

</script>

<template>
  <div class="sidebar-items">
    <sidebar-item
      v-for="i in 12" :key="i"
      class="sidebar-item"
    />
  </div>
</template>

<style lang="scss" scoped>
  .sidebar-item {
    user-select: none;
    cursor: pointer;
    transition: all 100ms ease-in-out;
    &:not(:last-child) {
      border-bottom: 1px solid rgba(white, 0.0375);
    }
    &:hover {
      background-color: rgba(white, 0.0375);
    }
    &:active {
      background-color: rgba(white, 0.075);
    }
  }
</style>