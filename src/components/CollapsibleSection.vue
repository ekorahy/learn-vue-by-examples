<script setup>
defineProps({
  title: String,
})
</script>

<template>
  <details>
    <summary>{{ title }}</summary>
    <section><slot></slot></section>
  </details>
</template>

<style>
details {
  padding: 0 16px;
}
</style>
