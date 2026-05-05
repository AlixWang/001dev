<script setup>
defineProps({
  value: {
    type: String,
    required: true
  },
  label: {
    type: String,
    required: true
  },
  note: {
    type: String,
    default: ''
  }
})
</script>

<template>
  <article class="metric-card">
    <strong>{{ value }}</strong>
    <span>{{ label }}</span>
    <small v-if="note">{{ note }}</small>
  </article>
</template>
