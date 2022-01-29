<script setup>
  import { inject } from '@vue/runtime-core';
  import HomeCostItem from './HomeCostItem.vue';

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

    <div class="cost__content">
      <HomeCostItem />
      <HomeCostItem />
      <HomeCostItem />
      <HomeCostItem />
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

  .cost__content {
    display: flex;
    flex-direction: column;
    gap: 1rem;
    margin-top: 1rem;
  }
</style>
