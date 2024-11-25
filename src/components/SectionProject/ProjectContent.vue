<script setup>
  defineProps({
    src: String,
    text: String,
  })
</script>

<template>
  <li class="project-list__item">
    <div class="img project-list__img">
      <img :src="src" alt>
    </div>
    <div class="project-list__desc">
      <p class="text project-list__text">{{ text }}</p>
      <img src="/arrow.svg" alt width="12" height="12">
    </div>
  </li>
</template>

<style scoped lang="scss">
  .project-list{
    &__item{
      width: 70%;
      flex-shrink: 0;
      overflow: hidden;
      position: relative;
      scroll-snap-align: center;
    }
    &__desc{
      width: 100%;
      position: absolute;
      bottom: .25rem;
      left: 0;
      padding: 0.6875rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      background: rgba(33, 37, 41, 0.5);
      z-index: 10;
    }
    &__text{
      color: var(--light-color);
    }
  }
</style>