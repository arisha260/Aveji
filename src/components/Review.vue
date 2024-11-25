<script setup>
  import Content from "@/components/SectionReviews/ReviewContent.vue";
</script>

<template>
  <section class="review">
    <div class="container review__container">
      <h1 class="title1 review__title">Отзывы</h1>
      <ul class="list-reset review__list review-list">
        <Content title="Игорь Антонов" text="Обратилась к Aveji по рекомендации. Команда сразу поняла, какой дизайн я хочу. Предоставили несколько вариантов и в течение недели сделали наброски. Итог понравился, все на высшем уровне."/>
        <Content title="Ольга Иванова" text="После пары заказов у компании Aveji убедилась, что за мебелью теперь только к ним. Абсолютно любые решения, в любых размерах и форм-факторе, то что нужно!"/>
        <Content title="Аркадий Макаров" text="Aveji — настоящие профессионалы своего дела. Быстро поняли мою задумку, сделали дизайн, согласовали и изготовили мебель. А потом еще и бесплатно все собрали на месте. Большое спасибо!"/>
      </ul>
    </div>
  </section>
</template>

<style scoped lang="scss">
  .review{
    margin-bottom: 3rem;
    &__title{
      margin-bottom: 1.25rem;
    }
  }

  .review-list{
    display: flex;
    flex-direction: column;
    gap: 1rem;
  }
</style>