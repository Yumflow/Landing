<template>
  <section class="section-products section">
    <div class="section-products__body container">
      <div class="section-products__header">
        <div class="section-products__subtitle">ПРОДУКТЫ</div>
        <div class="section-products__title">Которые улучшают взаимодействие клиентов с заведениями</div>
      </div>

      <div class="section-products__products">
        <Product />
      </div>
    </div>
  </section>
</template>

<script setup>
import Product from '@/modules/SectionProducts/components/Product.vue'
</script>

<style scoped lang="sass">
.section-products
  &__body
    display: flex
    flex-direction: column
    gap: 92px

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

  &__header
    max-width: 660px
    align-self: flex-end

  &__body
    //

  @media screen and (max-width: $breakpointMobile)
    &__body
      gap: 32px

    &__title
      font-size: 26px
      line-height: 32px

    &__subtitle
      font-size: 14px
      line-height: 18px
      margin-bottom: 8px
</style>