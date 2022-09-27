<template>
  <nav class="menu">
    <ul class="menu__list">
      <li class="menu__item">
        <router-link :to="{ name: 'index' }" class="menu__link">index</router-link>
      </li>
      <li class="menu__item">
        <router-link :to="{ name: 'canvas' }" class="menu__link">canvas</router-link>
      </li>
    </ul>
  </nav>
</template>

<style lang="sass" scoped>
.menu
  &__list
    list-style: none
    display: flex
    padding: 0
    margin: 0

  &__item
    margin: 0 20px

  &__link
    display: block
    padding: 10px
    font-size: 16px
</style>
