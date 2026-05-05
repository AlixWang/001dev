<script setup>
defineProps({
  label: {
    type: String,
    required: true
  },
  tone: {
    type: String,
    default: 'cyan'
  }
})
</script>

<template>
  <span class="stage-badge" :class="`stage-badge--${tone}`">{{ label }}</span>
</template>
