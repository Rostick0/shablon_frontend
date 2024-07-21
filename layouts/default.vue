<template>
  <div class="wrapper">
    <LayoutAside />
    <div class="wrapper__content">
      <LayoutHeader>
        <template #leftContent>
          <slot name="leftContent" />
        </template>
      </LayoutHeader>
      <main class="main">
        <slot />
      </main>
    </div>
  </div>
</template>

<script setup>
// console.log($)
</script>

<style lang="scss" scoped>
.wrapper {
  display: flex;

  &__content {
    flex-grow: 1;
  }
}

.main {
  flex-grow: 1;
}
</style>
