<script setup lang="ts">
import BlockSiteForm from '../components/BlockSiteForm.vue'

const backPage = () => window.history.back()
</script>

<template>
  <main class="space-y-3">
    <button @click="backPage"><- Back</button>
    <BlockSiteForm />
  </main>
</template>
