<script setup>
  import { ref } from '@vue/reactivity';
  import { provide } from '@vue/runtime-core';
  import HomeCard from '../components/home/HomeCard.vue';
  import HomeListCost from '../components/home/HomeListCost.vue';
  import HomeAddCpst from '../components/home/HomeAddCpst.vue';

  const stateModal = ref(false);
  provide('stateModal', stateModal);
</script>

<template>
  <HomeCard />
  <HomeListCost />
  <HomeAddCpst />
</template>
