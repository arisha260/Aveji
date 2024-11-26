<script setup>

</script>

<template>
  <nav class="nav">
    <a href="#" class="nav__site-logo">
      <img src="/site-logo.svg" alt="" width="26" height="28">
    </a>
    <ul class="list-reset nav__list">
      <li class="nav__item"><a href="#about" class="nav__link">О нас</a></li>
      <li class="nav__item"><a href="#project" class="nav__link">Проекты</a></li>
      <li class="nav__item"><a href="#" class="nav__link">Материалы</a></li>
      <li class="nav__item"><a href="#review" class="nav__link">Отзывы</a></li>
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
    @media (min-width: 64rem) {
      margin-left: auto;
      padding: 0;
      position: relative;
      width: auto;
      height: auto;
      flex-direction: row;
      transform: translate(0);
      gap: 12.9375rem;
    }
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
      position: relative;
      &::after{
        content: "";
        position: absolute;
        bottom: 0;
        left: 0;
        height: 2px;
        width: 0;
        background: var(--accent-color);
        transition: width .3s;
      }
      @media (hover: hover) {
        &:hover::after{
          width: 100%;
        }
      }
    }
    &.active{
      transform: translateX(0);
    }
    &__site-logo{
      @media (min-width: 64rem) {
        display: none;
      }
    }
  }
</style>