<script setup>
  import Content from "@/components/SectionOrder/OrderContent.vue";
  import IconAppStore from "@/components/icons/IconAppStore.vue";
  import IconGooglePlay from "@/components/icons/IconGooglePlay.vue";
</script>

<template>
  <section class="order">
    <div class="container order__container grid">
      <div class="img order__img">
        <img src="/order.png" alt>
      </div>
      <div class="order__content">
        <h1 class="title1 order__title">Хотите заказать проект?</h1>
        <p class="text order__text">Оставьте заявку, и мы вам перезвоним</p>
        <form class="form order__form">
          <div class="form__content">
            <Content type="text" id="name" labelfFor="name" labelText="Имя"/>
            <Content type="email" id="email" labelfFor="email" labelText="E-mail"/>
            <Content type="tel" id="tel" labelfFor="tel" labelText="Телефон"/>
          </div>
          <button class="btn-reset text form__btn">Отправить заявку</button>
        </form>
        <div class="order__download">
          <IconAppStore />
          <IconGooglePlay />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
  .order{
    margin-bottom: 3rem;
    @media (min-width: 78.75rem){
      margin-bottom: 8.25rem;
    }
    &__content{
      grid-column: 10/9 span;
    }
    &__title{
      margin-bottom: 1.25rem;
    }
    &__text{
      margin-bottom: 2rem;
    }
    &__download{
      display: flex;
      gap: .5rem;
    }
    &__img{
      display: none;
      @media (min-width: 78.75rem){
        display: block;
        grid-column: 8 span;
      }
    }
  }

  .form{
    width: 100%;
    &__content{
      margin-bottom: 1.25rem;
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }
    &__btn{
      margin-bottom: 1.75rem;
      padding: .75rem 1.25rem;
      color: var(--light-color);
      background: var(--main-color);
      transition: .3s;
      @media (hover: hover){
        &:hover{
          background-color: var(--accent-color);
        }
      }
      &:active{
        background-color: #9e9988;
      }
    }
  }
</style>