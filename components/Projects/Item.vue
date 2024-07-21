<template>
  <div class="project">
    <div class="project__image">
      <LazyNuxtImg
        class="project__img"
        :src="project?.preview"
        :alt="project?.name"
      />
    </div>
    <div class="project__title">{{ project?.title }}</div>
    <div class="project__date">
      {{ new Date(project?.created_ate).toLocaleDateString() }}
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  project: Object,
});
</script>

<style lang="scss" scoped>
.project {
  color: var(--white);
  position: relative;

  &__image {
    padding-top: 66%;
    position: relative;
  }

  &__img {
    border-radius: 8px;
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
  }

  &__title {
    background-color: rgba(0, 0, 0, 1);
    border-radius: 4px;
    padding: 2px 4px;
    position: absolute;
    left: 12px;
    bottom: 12px;
  }

  &__date {
    background-color: rgba(0, 0, 0, 1);
    border-radius: 4px;
    padding: 2px 4px;
    position: absolute;
    right: 12px;
    top: 12px;
  }
}
</style>
