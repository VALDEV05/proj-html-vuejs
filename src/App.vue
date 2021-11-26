<template>
  <div id="app">
    <SiteHeader :items="elementsNavbar"/>
    <SiteMain />
    <SiteFooter title="Footer"/>

  </div>
</template>

<script>
import SiteHeader from '@/components/SiteHeader.vue'
import SiteMain from '@/components/SiteMain.vue'
import SiteFooter from '@/components/SiteFooter.vue'

export default {
  name: 'App',
  data(){
    return{
      elementsNavbar:[
        {element : "home"},
        {element : "pages"},
        {element : "program"},
        {element : "tickets"},
        {element : "speakers"},
        {element : "papers"},
        {element : "blog"},
        {element : "shortcodes"},
      ]
    }
  },
  components: {
    SiteHeader,
    SiteMain,
    SiteFooter
  }
}
</script>

<style lang="scss">
@import "../node_modules/bootstrap/scss/bootstrap.scss";
@import '@/assets/style/variables.scss';
@import '@/assets/style/common.scss';
@import url('https://fonts.googleapis.com/css2?family=Bitter:ital,wght@1,600&family=Open+Sans:wght@300;400;500;600;700;800&display=swap');
</style>
