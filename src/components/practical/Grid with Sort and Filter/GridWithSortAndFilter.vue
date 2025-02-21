<script setup>
import GridComponent from './GridComponent.vue'
import { ref } from 'vue'

const searchQuery = ref('')
const gridColumns = ['name', 'power']
const gridData = [
  { name: 'Chuck Norris', power: Infinity },
  { name: 'Bruce Lee', power: 9000 },
  { name: 'Jackie Chan', power: 700 },
  { name: 'Jet Li', power: 8000 },
]
</script>

<template>
  <form id="search">Search <input type="text" name="query" v-model="searchQuery" /></form>

  <GridComponent :data="gridData" :columns="gridColumns" :filter-key="searchQuery"></GridComponent>
</template>
