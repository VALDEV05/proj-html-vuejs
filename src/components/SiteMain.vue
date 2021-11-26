<template>
  <div id="siteMain"> 
    <div id="jumbotron_socialNetwork" class="pt-5">
        <jumbotronSocialNetwork/>
    </div>
    <!-- /component jumbotron_socialNetwork -->
    <div id="section_card">
        <cardInfo />
    </div> 
    <!-- /component section_card -->

    <div id="jumbotron_countdown" class="jumbotronClass mt-5">
        <JumbotronCountdown/>
    </div>
    <!-- /component jumbotron_countdown -->
    <div id="speakers">
        <speakers/>
        
    </div>
    <!-- /# component speakers -->
    <div id="program">
        <programs />
    </div>
    <!-- /#component program -->
    <div id="googlemap" class="container">
        mappa
    </div>
    <!-- /#googlemap -->
    <div id="location">
        <location /> 
    </div>
    <!-- /#location -->
    <div id="recent_news">
        <recentNews/>
    </div>
    <!-- /#recent_news -->
    <div id="tickets">
        tickets
    </div>
    <!-- /#tickets -->
    <div id="presentation">
        presentation
    </div>
    <!-- /#presentation -->
    <div id="sponsor">
        sponsor
    </div>
    <!-- /#sponsor -->
  </div>
  <!-- /siteMain -->
</template>

<script>
import programs from '@/components/programs.vue'
import speakers from '@/components/speakers.vue'
import cardInfo from '@/components/cardInfo.vue'
import jumbotronSocialNetwork from '@/components/jumbotronSocialNetwork.vue'
import JumbotronCountdown from '@/components/jumbotronCountdown.vue'
import location from '@/components/location.vue'
import recentNews from '@/components/recentNews.vue'


export default {
    components:{
        speakers,
        programs,
        cardInfo,
        jumbotronSocialNetwork,
        JumbotronCountdown,
        location,
        recentNews

    },
    props:{
        title:String,
    },
}
</script>

<style  lang="scss">





</style>