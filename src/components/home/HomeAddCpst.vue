<script setup>
  import { inject } from '@vue/runtime-core';
  import Modal from '../modal/Modal.vue';

  const stateModal = inject('stateModal');

  const sendForm = () => {
    console.log('sendForm');
  };
</script>

<template>
  <Modal v-if="stateModal">
    <template v-slot:main>
      <form class="form" @submit.prevent="sendForm">
        <div class="form__group">
          <input type="number" placeholder="Agregar" class="form__input" />
        </div>
        <div class="form__botton">
          <button
            class="botton__cancel"
            @click="stateModal = false"
            type="button"
          >
            <i class="material-icons-outlined"> close </i>
          </button>
          <button type="submit" class="botton__send">
            <i class="material-icons-outlined"> done </i>
          </button>
        </div>
      </form>
    </template>
  </Modal>
</template>

<style scoped>
  .form__input {
    width: 100%;
    border: 1px solid #ccc;
    border-radius: 5px;
    padding: 1rem 0.5rem;
    outline: none;
  }

  .botton__cancel {
    background: #f44336;
    color: #fff;
    border: none;
    border-radius: 5px;
    padding: 0.5rem;
    outline: none;
  }

  .botton__send {
    background: #4caf50;
    color: #fff;
    border: none;
    border-radius: 5px;
    padding: 0.5rem;
    outline: none;
  }

  .form__botton {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 1rem;
  }
</style>
