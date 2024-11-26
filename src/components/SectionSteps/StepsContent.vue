<script setup>
  defineProps({
    title: String,
    text: String,
  })
</script>

<template>
  <li class="steps__item">
    <p class="title2 steps__item-title">{{ title }}</p>
    <p class="text steps__text">{{ text }}</p>
  </li>
</template>

<style lang="scss">
  .steps{
    &__item{
      display: flex;
      flex-direction: column;
      gap: 1rem;
      padding-bottom: 1.25rem;
      border-bottom: 1px solid var(--main-color);
      @media (min-width: 78.75rem){
        display: grid;
        grid-template-columns: repeat(6, 1fr);
      }
    }
    &__item-title{
      grid-column: 2 span;
    }
    &__text{
      grid-column: 4/3 span;
    }
  }
</style>