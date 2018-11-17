<template>
  <div>
    <HeaderTmp></HeaderTmp>
      <nuxt/>
    <FooterTmp></FooterTmp>
  </div>
</template>

<script>
import HeaderTmp from '~/components/HeaderTmp'
import FooterTmp from '~/components/FooterTmp'

export default {
  components: {
    HeaderTmp,
    FooterTmp
  }
}
</script>

<style>

</style>
