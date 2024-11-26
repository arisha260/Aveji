<script setup>
  defineProps({
    src: String,
    text: String,
  })
  const baseUrl = import.meta.env.BASE_URL;
</script>

<template>
  <li class="project-list__item">
    <div class="img project-list__img">
      <img :src="baseUrl + src" alt>
    </div>
    <div class="project-list__desc">
      <p class="text project-list__text">{{ text }}</p>
      <img src="/arrow.svg" alt width="12" height="12">
    </div>
    <a href="#" class="link"></a>
  </li>
</template>

<style scoped lang="scss">
  .project-list{
    &__item{
      height: 100%;
      width: 70%;
      flex-shrink: 0;
      overflow: hidden;
      position: relative;
      scroll-snap-align: center;
      font-size: 0;
      transition: .3s;
      @media (min-width: 48rem){
        flex: unset;
        width: auto;
        @media (hover: hover){
          &:hover{
            //scale: 1.1;
          }
          &:hover .project-list__desc{
            transform: translate(0);
          }
        }
      }
    }
    &__desc{
      width: 100%;
      position: absolute;
      bottom: 0;
      left: 0;
      padding: 0.6875rem;
      display: flex;
      align-items: center;
      justify-content: space-between;
      background: rgba(33, 37, 41, 0.5);
      z-index: 10;
      transition: .3s;
      @media (min-width: 48rem){
        transform: translateY(calc(100% + 1vh));
      }
    }
    &__text{
      color: var(--light-color);
    }
    &.link{
      position: absolute;
      inset: 0;
    }
    &__img{
      width: 100%;
      height: 100%;
      overflow: hidden;
    }
  }
</style>