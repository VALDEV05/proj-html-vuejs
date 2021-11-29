<template>
  <div id="siteMain"> 
    <div id="jumbotron_socialNetwork" class="pt-5">
        <jumbotronSocialNetwork title="conference on" titleLG="Social networks" buttonText="register online" :items="socialNetwork"/>
    </div>
    <!-- /component jumbotron_socialNetwork -->
    <div id="section_card">
        <cardInfo :items="cardInfodata"/>
    </div> 
    <!-- /component section_card -->

    <div id="jumbotron_countdown" class="jumbotronClass mt-5">
        <JumbotronCountdown/>
    </div>
    <!-- /component jumbotron_countdown -->
    <div id="speakers">
        <speakers title="Speakers" :subtitle="subtitle" :items="speakerCards"/>
        
    </div>
    <!-- /# component speakers -->
    <div id="program" class="mb-2">
        <programs title="programs" :days="programDays"  :items="dailySchedules"/>
    </div>
    <!-- /#component program -->
    <div id="googlemap">
        <mapComponent/>
    </div> 
    <!-- /#container mapComponent -->
    <div id="location" class="mt-2">
        <location :items="locationData" /> 
    </div>
    <!-- /#component location -->
    <div id="recent_news">
        <recentNews title="Recent News" viewFull="Read All News" :items="newsCardData"/>
    </div>
    <!-- /#component recent_news -->
    <div id="ticketSection">
        <ticketSection title="Tickets" button="book Now" :items="tickets"/>
    </div>
    <!-- /# component ticketSection -->
    <div id="presentationTwitter">
        <presentationTwitter titlePresentation="presentation" titleTwitter="twitter feed" :items="tweets" />
    </div>
    <!-- /#component presentationTwitter -->
    <div id="sponsor">
        <sponsor title="sponsors" subtitle="Maecenas faucibus mollis interdum. Nullam id dolor id nibh ultricies vehicula ut id elit" :items="sponsorBanners"/>
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
import mapComponent from '@/components/mapComponent.vue'


export default {
    components:{
        jumbotronSocialNetwork, 
        cardInfo,
        JumbotronCountdown,
        speakers,
        programs,
        mapComponent,
        location,
        recentNews,
        ticketSection,
        presentationTwitter,
        sponsor,
        
    },
    data(){
        return{
            socialNetwork:[
            {info: '23 - 26 may 2019'},
            {info: '/'},
            {info: 'sans francisco'},
            {info: '/'},
            {info: '8 speaker'},
            ],
            /* /Jumbotron Social data */
            cardInfodata:[
            {   
                index: 1,
                imageUrl:'trophy-solid.svg',
                altImage: 'trophy',
                title:'Who we Are',
                text:'Donec id elit non mi porta gravida at eget me tus. Sed posuere consectutyr estat lobo rtis. Cum sociis natoque.',
                link:'Learn More'
            },
            {   
                imageUrl:'bolt-solid.svg',
                altImage: 'bolt',
                title:'what we do',
                text:'Donec id elit non mi porta gravida at eget me tus. Sed posuere consectutyr estat lobo rtis. Cum sociis natoque.',
                link:'Learn More'
            },
            {   
                imageUrl:'question-solid.svg',
                altImage: 'question',
                title:'why us?',
                text:'Donec id elit non mi porta gravida at eget me tus. Sed posuere consectutyr estat lobo rtis. Cum sociis natoque.',
                link:'Learn More'
            }
            ],
            /* /cardInfo  data */
            speakerCards:[
                            {   
                                image:'speaker-6.jpg',
                                alt:'speaker-6',
                                name:'patrick spencer',
                                role:'S&P Analyzer'
                            },
                            {   
                                image:'speaker-5.jpg',
                                alt:'speaker-5',
                                name:'janet jones',
                                role:" Newyork Post's GM"
                            },
                            {   
                                image:'speaker-4.jpg',
                                alt:'speaker-4',
                                name:'Michael dover',
                                role: "Starbuck's CEO"
                            },
                            {   
                                image:'speaker-3.jpg',
                                alt:'speaker-3',
                                name:'Angelina holy',
                                role:"Maxii's Managar"
                            }
                            
            ],
            subtitle:'This conference run through all 4 days from 23-26 May 2016,We also provide free lunch and coffee break in each day',
            /* /speakers info */
            programDays:[
                {day:'Day 1', date:'23 May 2016', index:'1'},
                {day:'Day 2', date:'23 May 2030'},
                {day:'Day 3', date:'24 May 2030'},
                {day:'Day 4', date:'25 May 2030'},
                {day:'Day 5', date:'26 May 2030'},
                {day:'', date:''},
            ],
            dailySchedules:[{
                firstDay:{ 
                    hour:{
                        icon:'clock-regular.svg', 
                        hourly:'9:00-13:00'
                    },
                    location:{
                        icon:'location-arrow-solid.svg',
                        room:'room A'
                    }, 
                    speaker:{
                        icon:'user-solid.svg',
                        name:'Laurence francis',
                        image:'speaker-8.jpg'}, 
                    program:{
                        title:'Welcoming and introduction',
                        subtitle:'Vestibulum id ligula porta felis euismod semper. Nullam quis risus eget urna mollis ornare vel eu leo. Donec ullamcorper nella non metus auctor fringilla. Aenean lacinia bibendu, nulla sed cosectetur...'
                        }
                },
                }
            ],
            /* /program data */
            locationData:[
                {
                    title:'Location',
                    subtitle:'Gd building, grand conference room',
                    address:{
                        text:'11 GD Building, River Mail, New York, USA 8879',
                        icon:'location-arrow-solid-white.svg',
                        alt:'location'
                    },
                    check:'Check For accomodations here',
                    contacts:{
                        phone:{
                            icon:'phone-alt-solid-white.svg',
                            number:'+1-112-222-3344',
                            alt:'Phone White'
                        },
                        email:{
                            icon:'envelope-solid-white.svg',
                            address:'Contact@TheKeynoteTheme.com',
                            alt:'Email White'

                        }
                    }
                }
            ],
            /* /location data */
            newsCardData:[
                {
                    index:1,
                    imageUrl:'photodune-7770665-two-white-coffee-mug-with-diy-decoration-o (2).jpg',
                    subtitle:'03 Dec 2013 / 0 Comments',
                    title:'Sedial eiusmod tempor',
                    text:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente minima, excepturi officiis praesentium harum sunt neque explicabo ipsam odio sit?',
                    linkText:'Learn More'
                },
                {
                    index:2,
                    imageUrl:'photodune-8797753-multiethnic-people-with-startup-business-t (2).jpg',
                    subtitle:'03 Dec 2013 / 2 Comments',
                    title:'Donec luctus imperdiet',
                    text:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente minima, excepturi officiis praesentium harum sunt neque explicabo ipsam odio sit?',
                    linkText:'Learn More'
                },
                {
                    index:3,
                    imageUrl:'photodune-8522811-speaker-at-business-conference-and-present (2).jpg',
                    subtitle:'03 Dec 2013 / 0 Comments',
                    title:'Magna pars studiorum',
                    text:'Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente minima, excepturi officiis praesentium harum sunt neque explicabo ipsam odio sit?',
                    linkText:'Learn More'
                }
            ],
            /* /recentNews data */
            tickets:[
                        {
                            durationTicket:'One Day Pass',
                            priceTicket:'Free',
                            included:{
                                duration:'One Day Access',
                                beverage:'Coffee Break',
                                food:'Lunch (International Buffet)',
                                documentation:'Document Sheets',
                                bonus:'50USD Voucher For Next Event'
                            }, 
                        },
                        {
                            durationTicket:'four Day passes',
                            priceTicket:'750.00USD',
                            included:{
                                duration:'Four Day Access',
                                beverage:'Coffee Break',
                                food:'Lunch (International Buffet)',
                                documentation:'Document Sheets',
                                bonus:'100USD Voucher For Next Event'
                            }, 
                        },
                        {
                            durationTicket:'TWO Day Pass',
                            priceTicket:'580.00USD',
                            included:{
                                duration:'Two Day Access',
                                beverage:'Coffee Break',
                                food:'Lunch (International Buffet)',
                                documentation:'Document Sheets',
                                bonus:'70USD Voucher For Next Event'
                            }, 
                        }
            ],
            /* /tickets data */
            tweets:[
                {
                    logoUrl:'twitter-brands-celest.svg',
                    text: 'Stand out and be vibrant with some of the best bright and bold templates on @Envato Elements. And add a splash of c... https://t.co/jFrsnzEJK7',
                    date:'3 days ago'
                },
                {
                    logoUrl:'twitter-brands-celest.svg',
                    text: 'Stand out and be vibrant with some of the best bright and bold templates on @Envato Elements. And add a splash of c... https://t.co/jFrsnzEJK7',
                    date:'3 days ago'
                },
                {
                    logoUrl:'twitter-brands-celest.svg',
                    text: 'Stand out and be vibrant with some of the best bright and bold templates on @Envato Elements. And add a splash of c... https://t.co/jFrsnzEJK7',
                    date:'3 days ago'
                },
            ],
            /* /presentations */
            sponsorBanners:[
                {url: 'banner-1.jpg', alt: 'banner-1'},
                {url: 'banner-2.jpg', alt: 'banner-2'},
                {url: 'banner-3.jpg', alt: 'banner-3'},
                {url: 'banner-4.jpg', alt: 'banner-4'},
                {url: 'banner-5.jpg', alt: 'banner-5'},
                {url: 'banner-6.jpg', alt: 'banner-6'},
            ],
            /* /sponsors */
        }
    }
}
</script>

<style  lang="scss">





</style>