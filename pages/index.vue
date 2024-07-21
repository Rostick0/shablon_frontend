<template>
  <NuxtLayout>
    <template #leftContent> Главная </template>
    <div class="page-main container">
      <ProjectsList title="Последние проекты" :projects="data" />
      <NewProject />
    </div>
  </NuxtLayout>
</template>

<script setup>
const data = [
  {
    title: "Лес",
    created_ate: "07-22-2024 00:04:40",
    preview:
      "https://wallbox.ru/resize/1024x768/wallpapers/main/201440/f06101472e0e066.jpg",
  },
  {
    title: "Дом",
    created_ate: "07-22-2024 00:04:40",
    preview:
      "https://sun9-68.userapi.com/c628823/v628823296/21b22/FZ79LjaADa0.jpg",
  },
  {
    title: "Мост",
    created_ate: "07-22-2024 00:04:40",
    preview:
      "https://bareknucklepolitics.com/wp-content/uploads/2020/12/1289518-1536x864.jpg",
  },
];

useHead({
  title: "Главная",
});
</script>

<style lang="scss" scoped>
.page-main {
}
</style>
