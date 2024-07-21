<template>
  <div class="projects">
    <div class="title margin" v-if="title">{{ title }}</div>
    <div class="projects__list">
      <LazyProjectsItem
        v-for="project in projects"
        :key="project?.id"
        :project="project"
      />
    </div>
  </div>
</template>

<script setup>
const props = defineProps({
  projects: Array,
  title: String,
});
</script>

<style lang="scss" scoped>
.projects {
  &__list {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-gap: 20px;
  }
}
</style>
