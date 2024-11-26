<script setup>

</script>

<template>
  <section class="about" id="about">
    <div class="container about__container grid">
      <h2 class="title1 about__title">
        <span class="heading-mobile about__title-mob">О компании</span>
        <span class="heading-desktop about__title-desk">Более 5 лет создаем мебель для вашего комфорта</span>
      </h2>
      <div class="about__col col">
        <div class="about__text-container">
          <p class="text about__text">Мы — команда профессионалов, которые могут произвести любую мебель для вашего проекта, а также найти производственное решение любой задумки.</p>
          <p class="text about__text">Наша основная цель — реализовывать самые смелые задумки, и делать это качественно и аккуратно.</p>
          <p class="text about__text">В качестве материалов мы используем натуральные — стекло, дерево, бетон, камень, металл и эпоксидную смолу.</p>
        </div>
        <ul class="list-reset about__list">
          <li class="about__item">
            <p class="title2 about__item-title">1 год</p>
            <p class="text about__text">гарантии на всю продукцию</p>
          </li>
          <li class="about__item">
            <p class="title2 about__item-title">300+</p>
            <p class="text about__text">выполненных проектов</p>
          </li>
          <li class="about__item">
            <p class="title2 about__item-title">15 дней</p>
            <p class="text about__text">срок производства</p>
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
  .about{
    margin-bottom: 3rem;
    @media (min-width: 78.75rem){
      margin-bottom: 7.5rem;
    }
    &__container{
      align-items: baseline;
    }
    &__title{
      margin-bottom: 1.25rem;
      @media (min-width: 78.75rem){
        grid-column: 7 span;
      }
      &-mob{
        @media (min-width: 78.75rem){
          display: none;
        }
      }
      &-desk{
        @media (min-width: 78.75rem){
          display: block;
        }
      }
    }
    &__col{
      @media (min-width: 78.75rem){
        grid-column: 9/9 span;
      }
    }
    &__text-container{
      margin-bottom: 2rem;
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }
    &__list{
      max-width: 9.125rem;
      display: flex;
      flex-direction: column;
      gap: 1.25rem;

    }
  }
</style>