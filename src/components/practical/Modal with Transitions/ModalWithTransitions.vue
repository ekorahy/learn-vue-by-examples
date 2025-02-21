<script setup>
import { ref } from 'vue'
import ModalComponent from './ModalComponent.vue'

const showModal = ref(false)
</script>

<template>
  <button id="show-modal" @click="showModal = true">Show Modal</button>

  <Teleport to="body">
    <ModalComponent :show="showModal" @close="showModal = false">
      <template #header>
        <h3>Custom Header</h3>
      </template>
    </ModalComponent>
  </Teleport>
</template>
