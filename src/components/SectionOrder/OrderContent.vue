<script setup>
  defineProps({
    type: String,
    id: String,
    labelfFor: String,
    labelText: String,
  })
</script>

<template>
  <div class="form__group">
    <input class="input-reset input form__input" :type="type" :id="id" required>
    <label class="label text form__label" :for="labelfFor">{{ labelText }}</label>
  </div>
</template>

<style scoped lang="scss">
  .form{
    &__group{
      display: flex;
      flex-direction: column;
      position: relative;
    }
  }
</style>