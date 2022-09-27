<template>
  <page-layout>
    <template #header>
      <the-header />
    </template>
    <template #main>
      <router-view />
    </template>
    <template #footer>
      footer
    </template>
  </page-layout>
</template>

<script lang="ts" setup>
import PageLayout from 'src/components/app/PageLayout.vue'
import TheHeader from 'src/components/app/TheHeader.vue'
</script>
