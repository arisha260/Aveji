<script setup>
  import IconStaples from "@/components/icons/IconStaples.vue";

  defineProps({
    title: String,
    text: String,
  })
</script>

<template>
  <li class="review-list__item">
    <IconStaples class="review-list__icon"/>
    <h3 class="title2 review-list__title">{{ title }}</h3>
    <p class="text review-list__text">{{ text }}</p>
  </li>
</template>

<style scoped lang="scss">
  .review-list{
    &__item{
      height: 100%;
      padding: 2rem;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      flex-grow: 1;
      border: 1px solid var(--main-color);
      text-align: center;
    }
    &__icon{
      margin-bottom: 2rem;
    }
    &__title{
      margin-bottom: 1.25rem;
    }
  }
</style>