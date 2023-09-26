<template>
  <footer class="footer section">
    <div class="footer__body container">
      <div class="footer__header">
        <Image src="./images/logos/logo-with-title.svg" class="footer__logo" />

        <div class="footer__socials">
          <a href="https://t.me/yumflow" target="_blank" class="footer__socials-social">
            <Image src="./images/socials/telegram.svg" class="footer__socials-social" />
          </a>

          <a href="https://instagram.com/yumflow.by" target="_blank" class="footer__socials-social">
            <Image src="./images/socials/instagram.svg" class="footer__socials-social" />
          </a>
        </div>
      </div>

      <div class="footer__bottom">
        <div class="footer__bottom-copyright">© {{ currentYear }} Yumflow</div>
        <a href="mailto:contact@yumflow.biz" class="footer__bottom-email">contact@yumflow.biz</a>
      </div>
    </div>
  </footer>
</template>

<script setup>
import Image from '@/ui/Image.vue'

import { ref } from 'vue'

const currentYear = ref(new Date().getFullYear())
</script>

<style scoped lang="sass">
.footer
  margin-top: 164px

  &__header
    display: flex
    align-items: center
    justify-content: space-between
    padding-bottom: 24px
    margin-bottom: 24px
    border-bottom: 1px solid #dfe1ea

  &__logo
    height: 38px

  &__socials
    display: flex
    gap: 12px

    &-social
      height: 20px

  &__bottom
    color: #696d80
    display: flex
    align-items: center
    justify-content: space-between

    &-email
      //text-decoration: underline

  @media screen and (max-width: $breakpointMobile)
    margin-top: 72px

    &__logo
      height: 34px

    &__bottom
      font-size: 12px
</style>