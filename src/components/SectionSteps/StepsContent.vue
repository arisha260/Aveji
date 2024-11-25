<script setup>
  defineProps({
    title: String,
    text: String,
  })
</script>

<template>
  <li class="steps__item">
    <p class="title2">{{ title }}</p>
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
    }
  }
</style>