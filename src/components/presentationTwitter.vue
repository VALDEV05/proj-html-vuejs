<template>
  <div class="container">
      <div class="row">
          <div class="col-6 video my-4">
          <h1 class="text-uppercase">{{titlePresentation}}</h1>
          <img :src="require('@/assets/img/' + video.videoUrl)" alt="pres-control" v-for="video in videos" :key="video.videoUrl">
          </div>
      <div class="col-6 my-4">
          <h1 class="text-uppercase">{{titleTwitter}}</h1>
          <ul class="list-unstyled">
              <li class="tweet mb-4 d-flex" v-for="tweet in tweets" :key="tweet.logo">
                  <img :src="require('@/assets/img/' + tweet.logoUrl)"  style="height:50px; width:50px;" alt="">
                  <div id="text_message" class="ms-4">
                      <div class="text_message">
                        {{tweet.text}}
                      </div>
                      <div class="date mt-4">
                         {{tweet.date}}
                      </div>
                  </div>
              </li>
            </ul>
      </div>
      </div>
      
  </div>
</template>

<script>
export default {
    props:{
        titlePresentation:String,
        titleTwitter:String,
    },
    data(){
        return{
            videos:[
                {videoUrl:'presentation-control-bar.svg'}
            ],
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
            ]
        }
    }
}
</script>

<style lang="scss">
@import '@/assets/style/variables.scss';

.col-6.video{
    img{
        transform: scale(1.3);
    }
}
.text_message{
    font-size: 15px;
    color: $icon-gray;
    span{
        color: $scarlet-red-color;
    }
}
.date{
    font-family: 'Bitter', serif;
    color: $icon-gray;
}

</style>