<script setup lang="ts">
import BlockedSiteListItem from "./BlockedSiteListItem.vue"
</script>

<template>
    <article class="space-y-2">
        <section>
            <h3 class="text-lg">Blocked sites</h3>
        </section>
        <section>
            <ul>
                <BlockedSiteListItem site="https://www.google.com/" />
                <BlockedSiteListItem site="https://www.youtube.com/" />
            </ul>
        </section>
    </article>
</template>