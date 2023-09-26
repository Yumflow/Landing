<template>
  <header class="header">
    <div class="header__body container">
      <Image src="./images/logos/logo-with-title.svg" class="header__logo" />

      <div class="header__tabs">
        <div class="header__tab">Продукты</div>
        <div class="header__tab">Контакты</div>
        <div class="header__tab">Блог</div>
        <Button>Написать нам</Button>
      </div>
    </div>
  </header>
</template>

<script setup>
import Image from '@/ui/Image.vue'
import Button from '@/ui/Button.vue'
</script>

<style scoped lang="sass">
.header
  display: flex
  justify-content: center
  width: 100%
  padding: 24px 16px 16px

  &__body
    display: flex
    align-items: center
    justify-content: space-between
    width: 100%

  &__logo
    height: 54px

  &__tabs
    display: flex
    align-items: center
    gap: 40px

  &__tab
    font-size: 18px
    font-weight: 600
    line-height: 24px
    cursor: pointer

  @media screen and (max-width: $breakpointMobile)
    &__logo
      height: 36px

    &__tabs
      display: none
</style>