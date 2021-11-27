<template>
  <div id="background-sponsor"> 
      <div class="container">
            <div id="text-sponsor" class="text-center" v-for="(title, index) in titles" :key="index">
                <div class="title-sponsor text-uppercase fw-bold">
                    {{title.titleBg}}
                </div>
                <div class="subtitle-sponsor pt-3">
                    {{title.subTitle}}
                </div>
            </div>
            <div class="row mt-4 py-3">
                <div class="col-2 logo-sponsor" v-for="banner in banners" :key="banner.url">
                    <img :src="require('@/assets/img/' + banner.url)" :alt="banner.alt">

                </div>
            </div>
      
      </div>
      
  </div>
</template>

<script>
export default {
    data(){
        return{
            titles:[
                {titleBg: 'sponsor'},
                {subTitle: `Maecenas faucibus mollis interdum. Nullam id dolor id nibh ultricies vehicula ut id elit`}
            ],
            banners:[
                {url: 'banner-1.jpg', alt: 'banner-1'},
                {url: 'banner-2.jpg', alt: 'banner-2'},
                {url: 'banner-3.jpg', alt: 'banner-3'},
                {url: 'banner-4.jpg', alt: 'banner-4'},
                {url: 'banner-5.jpg', alt: 'banner-5'},
                {url: 'banner-6.jpg', alt: 'banner-6'},
            ]
        }
    }

}
</script>

<style lang="scss">
@import '@/assets/style/variables.scss';

#background-sponsor{
    background-color: #f6f6f6;
    width: 100vw;
    height: 500px;
    #text-sponsor{
        .title-sponsor{
            font-size: 50px;
        }
        .subtitle-sponsor{
            color: $icon-gray;
            width: 400px;
            margin: auto;
            
        }
    }
}
</style>