<template>
  <div id="app">
    <SiteHeader title="Header"/>
    <SiteMain title="Main"/>
    <SiteFooter title="Footer"/>

  </div>
</template>

<script>
import SiteHeader from '@/components/SiteHeader.vue'
import SiteMain from '@/components/SiteMain.vue'
import SiteFooter from '@/components/SiteFooter.vue'

export default {
  name: 'App',
  components: {
    SiteHeader,
    SiteMain,
    SiteFooter
  }
}
</script>

<style lang="scss">
@import '@/assets/style/common.scss';
</style>
