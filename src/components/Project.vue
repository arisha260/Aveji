<script setup>
  import Content from "@/components/SectionProject/ProjectContent.vue";
</script>

<template>
  <section class="project">
    <div class="container project__container">
      <h1 class="title1 project__title">Проекты</h1>
      <ul class="list-reset project__list project-list">
        <Content src="/project1.svg" text="Тумба под телевизор"/>
        <Content src="/project2.svg" text="Тумба под телевизор"/>
        <Content src="/project3.svg" text="Тумба под телевизор"/>
        <Content src="/project4.svg" text="Тумба под телевизор"/>
        <Content src="/project5.svg" text="Тумба под телевизор"/>
        <Content src="/project6.svg" text="Тумба под телевизор"/>
      </ul>
    </div>
  </section>
</template>

<style scoped lang="scss">
  .project{
    margin-bottom: 3rem;
    &__title{
      margin-bottom: 1.25rem;
    }
  }

  .project-list{
    gap: 1.25rem;
    overflow-x: auto;
    display: flex;
    align-items: stretch;
    scroll-padding: 1.25rem;
    scroll-snap-type: x mandatory;
  }
</style>