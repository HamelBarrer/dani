<script setup></script>

<template>
  <div class="card">
    <div class="card__header">
      <h2 class="card__title">Caja Principal</h2>
      <button class="card__bottonEdit">
        <i class="material-icons-outlined"> settings </i>
      </button>
    </div>
    <div class="card__content">
      <span class="card__value">$500.000</span>
    </div>
  </div>
</template>

<style scoped>
  .card__header {
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .card__title {
    text-transform: uppercase;
  }

  .card__bottonEdit {
    border: none;
    outline: none;
    background: none;
  }

  .card__content {
    display: flex;
    margin-top: 1rem;
    font-size: 1.5rem;
    justify-content: center;
    align-items: center;
  }
</style>
