<script setup>

</script>

<template>
  <button class="btn-reset burger">
    <span class="burger__line"></span>
  </button>
</template>

<style scoped lang="scss">
  .burger{
    display: block;
    position: relative;
    width: 25px;
    height: 12px;
    z-index: 10;
    color: var(--main-color);
    &__line{
      position: absolute;
      top: 50%;
      left: 0;
      height: 2px;
      width: 100%;
      background: currentColor;
      transform: translateY(-50%);
    }
    &::before, &::after{
      content: "";
      position: absolute;
      width: 100%;
      height: 2px;
      background: currentColor;
      transition: width .3s;
    }
    &::before{
      left: 0;
      top: 0;
    }
    &::after{
      bottom: 0;
      width: 50%;
      right: 0;
    }
    &.active::after{
      width: 100%;
    }
  }
</style>