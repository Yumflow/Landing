<template>
  <section class="section-contacts section">
    <div class="section-contacts__body container">
      <div class="section-contacts__subtitle">НАПИШИТЕ НАМ</div>

      <div class="section-contacts__title">Мы открыты для ваших идей</div>

      <div class="section-contacts__sections">
        <div class="section-contacts__section">
          <div class="section-contacts__section-title">Прокачайте свой бизнес</div>
          <div class="section-contacts__section-description">Если вы готовы к инновациям – мы ждём вашу заявку!</div>
          <Button class="section-contacts__section-button">Написать нам</Button>
        </div>

        <div class="section-contacts__section">
          <div class="section-contacts__section-title">Предложите вашу идею</div>
          <div class="section-contacts__section-description">Есть интересная идея для улучшения вашего бизнеса? Пишите – реализуем её вместе.</div>
          <Button class="section-contacts__section-button">Написать нам</Button>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import Button from '@/ui/Button.vue'
</script>

<style scoped lang="sass">
.section-contacts
  margin-top: 144px

  &__subtitle
    font-family: 'Ubuntu', sans-serif
    font-weight: 800
    font-size: 18px
    color: #3480f1
    margin-bottom: 16px

  &__title
    font-family: 'Ubuntu', sans-serif
    font-size: 48px
    font-weight: 600
    line-height: 54px
    letter-spacing: -0.24px

  &__sections
    margin-top: 88px
    display: flex
    justify-content: space-between
    gap: 80px

  &__section
    max-width: 500px

    &-title
      font-family: 'Ubuntu', sans-serif
      font-size: 28px
      font-weight: 600
      line-height: 32px
      margin-bottom: 8px

    &-description
      font-size: 20px
      font-weight: 400
      line-height: 30px
      margin-bottom: 48px

  @media screen and (max-width: $breakpointMobile)
    margin-top: 72px

    &__title
      font-size: 26px
      line-height: 32px

    &__subtitle
      font-size: 14px
      line-height: 18px
      margin-bottom: 8px

    &__sections
      flex-direction: column
      gap: 32px
      margin-top: 32px

    &__section
      &-title
        font-size: 20px
        line-height: 28px

      &-description
        font-size: 15px
        line-height: 22px
        margin-bottom: 20px
</style>