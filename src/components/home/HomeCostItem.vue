<script setup>
  import { inject } from '@vue/runtime-core';

  const editCost = inject('editCost');
</script>

<template>
  <div class="cost__item" @click="editCost = !editCost">
    <span class="cost__value">$127.000</span>
    <span class="cost__date">12/12/2021</span>
  </div>
</template>

<style scoped>
  .cost__item {
    display: flex;
    justify-content: space-between;
    align-items: center;
    background-color: #f8f8f8;
    padding: 1rem;
    border-radius: 0.5rem;
  }
</style>
