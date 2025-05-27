<script setup lang="ts">
defineProps<{
  site: string
}>()
</script>

<template>
    <div class="flex justify-between items-center p-2 border-b border-b-black">
        <p class="text-base">{{ site }}</p>
        <div class="flex space-x-3">
            <button class="cursor-pointer"><i class="pi pi-pencil text-[#007bff] text-base"></i></button>
            <button class="cursor-pointer"><i class="pi pi-trash text-[#ff0000] text-base"></i></button>
        </div>
    </div>
</template>