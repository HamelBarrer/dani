<script setup></script>

<template>
  <div class="modal">
    <div class="modal__content">
      <slot name="main"> </slot>
    </div>
  </div>
</template>

<style scoped>
  .modal {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(244, 244, 244, 0.8);
    z-index: 10;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .modal__content {
    background: #fff;
    width: max-content;
    height: max-content;
    border-radius: 5px;
    padding: 1rem;
    box-shadow: 0 12px 28px 0 rgba(0, 0, 0, 0.2), 0 2px 4px 0 rgba(0, 0, 0, 0.1),
      inset 0 0 0 1px rgba(255, 255, 255, 0.5);
  }
</style>
