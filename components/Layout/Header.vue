<template>
  <div class="header">
    <div class="header__left">
      <slot name="leftContent" />
    </div>
    <div class="header__right">
      <div class="header-user">
        <span>Привет, Админ</span>
        <div class="header-user__avatar">А</div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.header {
  background-color: var(--blue-light);
  color: var(--white);
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 16px;

  &-user {
    display: flex;
    align-items: center;
    column-gap: 4px;

    &__avatar {
      background-color: var(--dark);
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-shrink: 0;
      font-weight: 600;
      width: 40px;
      height: 40px;
    }
  }
}
</style>
