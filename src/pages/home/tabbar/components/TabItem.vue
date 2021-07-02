<script setup>

import { toRefs } from "vue";

const emit = defineEmit(['click', 'close']);

const props = defineProps({
  active: Boolean
});

</script>

<template>
  <div class="tab-item" :class="{ 'active' : props.active }" style="height: 100%;">
    <div class="wrapper px-2 d-flex flex-row align-center" style="height: 100%;" @click.self="$emit('click')">

      <span class="text-caption" @click="$emit('click')">
        ApiName
      </span>

      <v-btn v-if="active" text icon class="ms-1" size="auto" style="padding: 1px" @click="$emit('close')">
        <v-icon size="12">mdi-close</v-icon>
      </v-btn>

    </div>
  </div>
</template>

<style lang="scss" scoped>
  .tab-item {
    cursor: pointer;
    user-select: none;
  }
  .tab-item.active {
    background-color: rgba(white, 0.0325);
  }
  .tab-item:not(:last-child) {
    border-right: 1px solid rgba(white, 0.075);
  }
</style>