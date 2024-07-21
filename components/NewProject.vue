<template>
  <div class="new">
    <div class="new__title title margin">Создать новый проект</div>
    <div class="new__buttons">
      <UiButton>Новый проект</UiButton>
      <UiButton>Загрузить архив</UiButton>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.new {
  &__buttons {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-gap: 20px;
    margin: 0 auto;
    max-width: 420px;
  }
}
</style>
