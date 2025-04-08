<script setup lang="ts">
import { ref } from 'vue';

const clicks = ref(0)

function incClicks() {
  clicks.value += 1
}
</script>

<template>
  <div>
    <div><q-btn color="primary" label="Primary" @click="incClicks" /></div>
    <div>clicks: {{ clicks }}</div>
  </div>
</template>