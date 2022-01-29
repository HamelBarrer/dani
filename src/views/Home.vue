<script setup>
  import { ref } from '@vue/reactivity';
  import { provide } from '@vue/runtime-core';
  import HomeCard from '../components/home/HomeCard.vue';
  import HomeListCost from '../components/home/HomeListCost.vue';
  import HomeAddCpst from '../components/home/HomeAddCpst.vue';
  import HomeEditCost from '../components/home/HomeEditCost.vue';

  const stateModal = ref(false);
  const editCost = ref(false);

  provide('stateModal', stateModal);
  provide('editCost', editCost);
</script>

<template>
  <HomeCard />
  <HomeListCost />
  <HomeAddCpst />
  <HomeEditCost />
</template>
