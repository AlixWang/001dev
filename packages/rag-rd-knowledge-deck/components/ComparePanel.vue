<script setup>
defineProps({
  title: {
    type: String,
    required: true
  },
  type: {
    type: String,
    default: 'bad'
  }
})
</script>

<template>
  <section class="compare-panel" :class="`compare-panel--${type}`">
    <header>{{ title }}</header>
    <div class="compare-panel__body">
      <slot />
    </div>
  </section>
</template>
