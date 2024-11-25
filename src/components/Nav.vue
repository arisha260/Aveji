<script setup>

</script>

<template>
  <nav class="nav">
    <a href="#" class="nav__site-logo">
      <img src="/site-logo.svg" alt="" width="26" height="28">
    </a>
    <ul class="list-reset nav__list">
      <li class="nav__item"><a href="#" class="nav__link">О нас</a></li>
      <li class="nav__item"><a href="#" class="nav__link">Проекты</a></li>
      <li class="nav__item"><a href="#" class="nav__link">Материалы</a></li>
      <li class="nav__item"><a href="#" class="nav__link">Отзывы</a></li>
    </ul>
    <a href="tel:+79999999999" class="nav__link">+7 999 999 99 99</a>
  </nav>
</template>

<style scoped lang="scss">
  .nav{
    position: fixed;
    top: 0;
    right: 0;
    padding: 2rem;
    width: 300px;
    height: 100vh;
    transform: translateX(calc(100% + 5vw));
    display: flex;
    justify-content: flex-start;
    align-items: flex-start;
    flex-direction: column;
    gap: 2rem;
    background: var(--light-color);
    transition: transform .5s;
    z-index: 10;
    &__list{
      display: flex;
      flex-direction: column;
      gap: 0.5rem;
    }
    &__link{
      font-family: var(--font-family);
      font-weight: var(--fw-400);
      font-size: 18px;
      color: var(--main-color);
    }
    &.active{
      transform: translateX(0);
    }
  }
</style>