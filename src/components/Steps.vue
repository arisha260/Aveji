<script setup>
  import Content from "@/components/SectionSteps/StepsContent.vue";
</script>

<template>
  <section class="steps">
    <div class="container steps__container grid">
      <h1 class="title1 steps__title">Как мы работаем</h1>
      <div class="steps__col col">
        <p class="text steps__text">Алгоритм работы с нами для удобства и понимания проекта</p>
        <ul class="list-reset steps__list">
          <Content title="Идея" text="Клиент приходит к нам с идеей. Это может быть изображение/ эскиз или другой референс. А мы думаем над тем, как это реализовать, делаем технические чертежи и предлагаем решения по материалам."/>
          <Content title="Техническое задание" text="Вместе с клиентом формулируем корректное ТЗ, которое включает в себя визуализацию изделия, эскизный чертёж с габаритами, информацию по материалам и отделке, срок реализации проекта и другие обязательные пункты."/>
          <Content title="Коммерческое предложение" text="Предпочтительно используем натуральные материалы. Но любую смету можем оптимизировать, упростив материалы или конструктив. Сможем подстроиться под бюджет клиента и согласуем коммерческое предложение"/>
          <Content title="Подготовка рабочего проекта" text="Создадим рабочую документацию и чертежи. Это фундамент качественного производства. На этом этапе утверждаем с клиентом все габариты и материалы, чертежи и приступаем к производству."/>
          <Content title="Производство и монтаж" text="Производство занимает от 15 рабочих дней, в зависимости от сложности и объёма. Монтажом тоже занимаемся самостоятельно. Ведь мы это сделаем быстро и аккуратно."/>
        </ul>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
  .steps{
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
    }
    &__col{
      gap: 1.75rem;
      @media (min-width: 78.75rem){
        grid-column: 9/9 span;
      }
    }
    &__list{
      display: flex;
      flex-direction: column;
      gap: 1.25rem;
    }
  }
</style>