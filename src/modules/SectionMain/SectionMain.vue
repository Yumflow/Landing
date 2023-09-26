<template>
  <section class="section-main section">
    <div class="section-main__body container">
      <div class="section-main__title">Yumflow.<br>Помогаем заведениям<br>стать лучше</div>

      <div class="section-main__description">
        Цифровое решение для вкусного успеха. Мы преображаем пищевые заведения с помощью инновационных технологий и стратегий для улучшения эффективности и удовлетворения клиентов.
      </div>
    </div>

    <Image src="./images/logos/logo.svg" class="section-main__background" />
  </section>
</template>

<script setup>
import Image from '@/ui/Image.vue'
</script>

<style scoped lang="sass">
.section-main
  padding: 124px 16px 164px
  position: relative

  &__body
    display: flex
    flex-direction: column

  &__title
    font-family: 'Ubuntu', sans-serif
    font-size: 80px
    font-weight: 600
    line-height: 90px
    margin-bottom: 92px
    letter-spacing: -0.8px

  &__description
    max-width: 660px
    align-self: flex-end
    font-size: 22px
    font-weight: 400
    line-height: 30px

  &__background
    pointer-events: none
    position: absolute
    bottom: -200px
    left: -150px
    height: 740px
    color: #FFE4A7
    z-index: -1

  @media screen and (max-width: $breakpointMobile)
    padding: 68px 16px 72px

    &__title
      font-size: 32px
      line-height: 38px
      letter-spacing: -0.17px

    &__description
      max-width: 280px
      font-size: 15px
      line-height: 22px

    &__background
      bottom: 20px
      height: 400px
</style>