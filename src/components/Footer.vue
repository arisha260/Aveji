<script setup>

</script>

<template>
  <footer class="footer">
    <div class="container footer__container">
      <ul class="list-reset footer__list footer-list">
        <li class="footer__item"><a href="#" class="large-text footer-list__link">вконтакте</a></li>
        <li class="footer__item"><a href="#" class="large-text footer-list__link">телеграм</a></li>
      </ul>
      <div class="footer__policy">
        <a href="#" class="text">Политика конфеденциальности</a>
        <a href="#" class="text">Оплата и доставка</a>
      </div>
      <div class="large-text footer__copy">
        <span>© 2023 Aveji</span>
        <span>Все права защищены</span>
      </div>
    </div>
  </footer>
</template>

<style scoped lang="scss">
  .footer{
    margin-bottom: 1.25rem;
    &__container{
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: center;
      gap: 1.75rem;
      @media (min-width: 48rem){
        justify-content: space-between;
        align-items: flex-end;
      }
    }
    &__policy{
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      @media (min-width: 48rem){
        order: 1;
      }
      @media (min-width: 64rem){
        flex-direction: row;
        gap: 0.5rem;
        :first-child::after{
          content: "/";
          margin-left: 0.5rem;
        }
      }
    }
    &__copy{
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      @media (min-width: 48rem){
        align-items: flex-start;
      }
    }
  }

  .footer-list{
    display: flex;
    gap: 40px;
    @media (min-width: 48rem){
      order: 2;
    }
    &__link{
      text-transform: uppercase;
    }
  }
</style>