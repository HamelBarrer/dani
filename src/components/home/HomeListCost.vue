<script setup>
  import { inject } from '@vue/runtime-core';

  const stateModal = inject('stateModal');
</script>

<template>
  <div class="cost">
    <div class="cost__header">
      <h2 class="cost__title">Lista Precios</h2>
      <button class="cost__addCost" @click="stateModal = !stateModal">
        <i class="material-icons-outlined"> add </i>
      </button>
    </div>
  </div>
</template>

<style scoped>
  .cost {
    margin-top: 1rem;
  }

  .cost__header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid #ccc;
  }
  .cost__title {
    text-transform: uppercase;
  }

  .cost__addCost {
    border: none;
    outline: none;
    background: none;
  }
</style>
