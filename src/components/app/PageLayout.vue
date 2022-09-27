<template>
  <div class="page-layout">
    <slot name="header" />

    <main class="page-layout__main">
      <div class="page-layout__inner">
        <slot name="main" />
      </div>
    </main>

    <slot name="footer" />
  </div>
</template>

<style lang="sass" scoped>
.page-layout
  height: 100vh
  display: flex
  flex-direction: column

  &__main
    width: 100%
    max-width: 800px
    margin: 0 auto
    flex: 1
    display: flex
    align-items: center

  &__inner
    width: 100%
</style>
