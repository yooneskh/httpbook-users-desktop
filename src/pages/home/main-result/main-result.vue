<script setup>

import { ref } from "vue";


const result = ref([
  {
    _id: '123123123',
    name: 'Yoones Khoshghadam',
    lastnAme: 'asdfasdf'
  },
  {
    _id: '123123123',
    name: 'Yoones Khoshghadam',
    lastnAme: 'asdfasdf'
  },
  {
    _id: '123123123',
    name: 'Yoones Khoshghadam',
    lastnAme: 'asdfasdf'
  },
  {
    _id: '123123123',
    name: 'Yoones Khoshghadam',
    lastnAme: 'asdfasdf'
  }
]);

</script>

<template>
  <pre class="main-result pa-1">{{ result }}</pre>
</template>

<style lang="scss" scoped>
  .main-result {
    border-left: 1px solid rgba(white, 0.075);
    font-family: monospace;
    font-size: 13px;
  }
</style>