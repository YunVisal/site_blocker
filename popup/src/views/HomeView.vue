<script setup lang="ts">
import BlockedSiteList from "../components/BlockedSiteList.vue"
import {useRouter} from 'vue-router'

const router = useRouter()

const navigateToPage = () => {
  router.push('/form')
}
</script>

<template>
  <main>
    <article class="flex justify-center">
      <button 
        class="p-2 bg-[#007bff] text-white rounded-md cursor-pointer"
        @click="navigateToPage"
      >
        Block this site
      </button>
    </article>
    <BlockedSiteList />
  </main>
</template>
