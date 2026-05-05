<script setup>
defineProps({
  kicker: {
    type: String,
    default: ''
  },
  title: {
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
  <div class="flow-node" :class="`flow-node--${tone}`">
    <div v-if="kicker" class="flow-node__kicker">{{ kicker }}</div>
    <div class="flow-node__title">{{ title }}</div>
  </div>
</template>
