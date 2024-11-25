<script setup>
  import Nav from "@/components/Nav.vue";
  import Burger from "@/components/Burger.vue";
  import {ref} from "vue";

  const activeBurger = ref(false);
  const activeNav = ref(false);

  const toggleActive = () => {
    activeBurger.value = !activeBurger.value;
    activeNav.value = !activeNav.value;
    if (activeBurger.value) {
      document.body.classList.add("active");
    } else{
      document.body.classList.remove("active");
    }
  }

</script>

<template>
  <header class="header">
    <div class="container header__container">
      <img src="/site-logo.svg" alt="" width="26" height="28" />
      <Nav class="header__nav" :class="{ active:activeNav }"/>
      <Burger class="header__burger" @click="toggleActive" :class="{ active:activeBurger }"/>
    </div>
  </header>
</template>

<style scoped lang="scss">
  .header{
    padding: 0.5rem 0 1.25rem 0;
    &__container{
      display: flex;
      align-items: center;
      justify-content: space-between;
    }
  }
</style>