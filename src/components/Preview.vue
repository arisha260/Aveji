<script setup>

</script>

<template>
  <section class="preview">
    <div class="container preview__container grid">
      <h1 class="title preview__title">Эксклюзивная и нестандартная мебель для дома</h1>
      <p class="text preview__text">Мы можем произвести любую мебель для вашего проекта и найти производственное решение любой задумки.</p>
      <a href="#" class="button preview__btn">заказать проект</a>
      <div class="img preview__img">
        <img src="/preview.png" alt>
      </div>
      <div class="img desktop">
        <img src="/preview-small.png" alt>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
  .preview{
    margin-bottom: 3rem;
    @media (min-width: 78.75rem){
      margin-bottom: 7.5rem;
    }
    &__title{
      margin-bottom: 1.25rem;
      @media (min-width: 78.75rem){
        grid-column: 10 span;
        margin: 0;
      }
    }
    &__text{
      margin-bottom: 1.5rem;
      @media (min-width: 78.75rem){
        grid-row: 2 / 3;
        grid-column: 6 span;
        margin: 0;
      }
    }
    &__btn{
      margin-bottom: 1.5rem;
      @media (min-width: 78.75rem){
        margin-bottom: 0;
        grid-column-end: 19;
        grid-column-start: 17;
      }
    }
    &__img{
      width: 100%;
      height: 16.25rem;
      @media (min-width: 48rem){
        height: 30rem;
      }
      @media (min-width: 78.75rem){
        height: auto;
        grid-row: 2 span;
        grid-column-start: 10;
        grid-column-end: 19;
      }
    }
  }
</style>