<template>
  <main class="main">
    <AppHeader />
    <SectionMain />
    <SectionProducts />
    <SectionContacts />
    <AppFooter />
  </main>
</template>

<script setup>
import AppHeader from '@/modules/AppHeader'
import SectionMain from '@/modules/SectionMain'
import SectionProducts from '@/modules/SectionProducts'
import AppFooter from '@/modules/AppFooter'
import SectionContacts from '@/modules/SectionContacts'
</script>

<style lang="sass">
.main
  display: flex
  flex-direction: column
  padding-bottom: 40px
</style>