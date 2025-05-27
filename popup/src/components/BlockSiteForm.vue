<script setup lang="ts">
import Toggle from '@vueform/toggle'
import { ref } from 'vue'

const isForever = ref(true)
</script>

<style src="@vueform/toggle/themes/default.css"></style>

<template>
    <article class="space-y-2">
        <section>
            <form class="space-y-2">
                <div class="space-y-1">
                    <label for="sites_name" class="block text-base">Sites to be blocked:</label>
                    <input 
                        type="text" 
                        id="sites_name" 
                        name="sites_name" 
                        class="w-full p-1 border border-black rounded-md outline-none text-base"
                    />
                </div>
                <div class="flex justify-between items-center">
                    <label for="is_forever" class="block text-base">Block forever:</label>
                    <Toggle v-model="isForever" />
                </div>
                <div class="space-y-1" v-if="!isForever">
                    <label for="block_duration" class="block text-base">Block duration:</label>
                    <input 
                        type="date" 
                        id="block_duration" 
                        name="block_duration" 
                        class="w-full p-1 border border-black rounded-md outline-none text-base"
                    />
                </div>
                <div class="w-1/4 m-auto">
                    <input 
                        type="submit"
                        value="Block"
                        class="w-full p-2 bg-[#007bff] text-white rounded-md cursor-pointer text-base"
                    />
                </div>
            </form>
        </section>
    </article>
</template>