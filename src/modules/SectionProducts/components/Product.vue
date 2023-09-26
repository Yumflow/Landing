<template>
  <div class="product">
    <Image src="./images/phone.png" class="product__image" />

    <div class="product__info">
      <Image src="./images/telegram-bot.svg" class="product__icon" />

      <div class="product__text">
        <div class="product__title">Telegram-бот</div>

        <div class="product__description">
          Интеграция заведения в Telegram-бота позволяет клиентам делать заказы предварительно, а также улучшает обратную связь.
        </div>
      </div>

      <Button is-primary class="product__button">Смотреть</Button>
    </div>
  </div>
</template>

<script setup>
import Image from '@/ui/Image.vue'
import Button from '@/ui/Button.vue'
</script>

<style scoped lang="sass">
.product
  background-color: #f8f8f9
  border-radius: 24px
  display: flex
  gap: 150px
  padding-left: 81px
  padding-right: 52px
  width: 100%

  &__image,
  &__info
    padding-top: 48px

  &__image
    max-height: 508px

  &__info
    display: flex
    flex-direction: column
    gap: 32px

  &__icon
    height: 64px
    width: 64px

  &__title
    font-family: 'Ubuntu', sans-serif
    font-size: 28px
    font-weight: 600
    line-height: 32px
    margin-bottom: 8px

  &__description
    font-size: 20px
    font-weight: 400
    line-height: 30px

  &__button
    width: fit-content

  @media screen and (max-width: $breakpointMobile)
    flex-direction: column-reverse
    padding-left: 24px
    padding-right: 24px
    gap: 24px

    &__info
      padding: 24px 0
      gap: 24px

    &__image
      padding-top: 0

    &__title
      font-size: 20px
      line-height: 28px

    &__description
      font-size: 15px
      line-height: 22px
</style>