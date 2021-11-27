<template>
  <div id="siteMain"> 
    <div id="jumbotron_socialNetwork" class="pt-5">
        <jumbotronSocialNetwork title="conference on" titleLG="Social networks"/>
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
        <speakers title="Speakers"/>
        
    </div>
    <!-- /# component speakers -->
    <div id="program" class="mb-2">
        <programs />
    </div>
    <!-- /#component program -->
    <!-- <div id="googlemap">
        <mapComponent/>
    </div> -->
    <!-- /#container mapComponent -->
    <div id="location" class="mt-2">
        <location /> 
    </div>
    <!-- /#component location -->
    <div id="recent_news">
        <recentNews/>
    </div>
    <!-- /#component recent_news -->
    <div id="ticketSection">
        <ticketSection/>
    </div>
    <!-- /# component ticketSection -->
    <div id="presentationTwitter">
        <presentationTwitter titlePresentation="presentation" titleTwitter="twitter feed"/>
    </div>
    <!-- /#component presentationTwitter -->
    <div id="sponsor">
        <sponsor />
    </div>
    <!-- /#component sponsor -->
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
import ticketSection from '@/components/ticketSection.vue'
import presentationTwitter from '@/components/presentationTwitter.vue'
import sponsor from '@/components/sponsor.vue'
//import mapComponent from '@/components/mapComponent.vue'


export default {
    components:{
        speakers,
        programs,
        cardInfo,
        jumbotronSocialNetwork,
        JumbotronCountdown,
        location,
        recentNews,
        ticketSection,
        presentationTwitter,
        sponsor,
        //mapComponent,
    },
}
</script>

<style  lang="scss">





</style>