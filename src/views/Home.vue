<script setup>
  import { ref } from '@vue/reactivity';
  import { provide } from '@vue/runtime-core';
  import HomeCard from '../components/home/HomeCard.vue';
  import HomeListCost from '../components/home/HomeListCost.vue';
  import HomeAddCpst from '../components/home/HomeAddCpst.vue';
  import HomeEditCost from '../components/home/HomeEditCost.vue';
  import HomeEditCostBox from '../components/home/HomeEditCostBox.vue';

  const stateModal = ref(false);
  const editCost = ref(false);
  const editCostBox = ref(false);

  provide('stateModal', stateModal);
  provide('editCost', editCost);
  provide('editCostBox', editCostBox);
</script>

<template>
  <HomeCard />
  <HomeListCost />
  <HomeAddCpst />
  <HomeEditCost />
  <HomeEditCostBox />
</template>
