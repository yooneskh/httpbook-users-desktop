<script setup>

</script>

<template>
  <div class="selector pa-4 text-body-1 align-center font-weight-bold">

    Project

    <v-spacer />

    <v-btn size="x-small" flat icon elevation="0">
      <v-icon size="x-small">mdi-cog</v-icon>
    </v-btn>

  </div>
</template>

<style lang="scss" scoped>
  .selector {
    transition: all 100ms ease-in-out;
    cursor: pointer;
    user-select: none;
    display: flex;
    border-bottom: 1px solid rgba(white, 0.075);
    &:hover {
      background: rgba(white, 0.075);
    }
    &:active {
      background: rgba(white, 0.15);
    }
  }
</style>