<template>
  <div class="index-page">
    <div class="index-page__col">
      <app-canvas title="first" />
    </div>
    <div class="index-page__col">
      <app-canvas title="second" />
    </div>
  </div>
</template>

<script lang="ts" setup>
import AppCanvas from 'src/components/app/Canvas.vue'
</script>

<style lang="sass" scoped>
.index-page
  width: 100%
  display: flex

  &__col
    width: 50%
</style>
