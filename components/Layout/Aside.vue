<template>
  <div class="aside">
    <div class="aside__logo">Shablon</div>
    <div class="aside-menu">
      <NuxtLink class="aside-menu__item" to="/projects">
        <svg
          width="24"
          height="24"
          viewBox="0 0 16 16"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <rect x="6" y="10" width="1" height="4" fill="white" />
          <rect x="10" y="6" width="3" height="1" fill="white" />
          <rect x="7" y="13" width="6" height="1" fill="white" />
          <path
            d="M14 6H13V14V14C13.5523 14 14 13.5523 14 13V6Z"
            fill="white"
          />
          <path
            d="M3 2.5H9.5V8.5C9.5 9.05228 9.05228 9.5 8.5 9.5H2.5V3C2.5 2.72386 2.72386 2.5 3 2.5Z"
            stroke="white"
          />
        </svg>
        <span>Мои проекты</span>
      </NuxtLink>
      <NuxtLink class="aside-menu__item" to="/projects">
        <svg
          width="24"
          height="24"
          viewBox="0 0 16 16"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <rect x="2.5" y="2.5" width="4" height="4" rx="0.5" stroke="white" />
          <path
            d="M10 2.5H13C13.2761 2.5 13.5 2.72386 13.5 3V6C13.5 6.27614 13.2761 6.5 13 6.5H10C9.72386 6.5 9.5 6.27614 9.5 6V3C9.5 2.72386 9.72386 2.5 10 2.5Z"
            stroke="white"
          />
          <rect x="2.5" y="9.5" width="4" height="4" rx="0.5" stroke="white" />
          <rect x="9.5" y="9.5" width="4" height="4" rx="0.5" stroke="white" />
        </svg>
        <span>Шаблоны проектов</span>
      </NuxtLink>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.aside {
  background-color: var(--dark);
  color: var(--white);
  min-height: 100vh;

  &__logo {
    font-size: 24px;
    font-weight: 700;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 10px;
    min-height: 72px;
  }

  &-menu {
    display: flex;
    flex-direction: column;
    row-gap: 8px;
    padding: 0 10px;

    &__item {
      border-radius: 4px;
      color: var(--white);
      display: flex;
      align-items: center;
      column-gap: 8px;
      transition: 0.3s;
      padding: 10px;

      &:hover {
        background-color: var(--blue-light);
      }

      span {
        line-height: 1;
      }
    }
  }
}
</style>
