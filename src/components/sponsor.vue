<template>
  <div id="background-sponsor"> 
      <div class="container">
            <div id="text-sponsor" class="text-center">
                <div class="title-sponsor text-uppercase fw-bold">
                    sponsor
                </div>
                <div class="subtitle-sponsor pt-3">
                    Maecenas faucibus mollis interdum. Nullam id dolor <br>id nibh ultricies vehicula ut id elit.
                </div>
            </div>
            <div class="row mt-4 py-3">
                <div class="col-2 logo-sponsor" v-for="banner in banners" :key="banner">
                    <img :src="banner.url" alt="">
                    <p>{{banner.url}}</p>

                </div>
            </div>
      
      </div>
      
  </div>
</template>

<script>
export default {
    data(){
        return{
            banners:[
                {url: '@/assets/img/banner-1.jpg', alt: 'banner-1'},
                {url: '@/assets/img/banner-2.jpg', alt: 'banner-2'},
                {url: '@/assets/img/banner-3.jpg', alt: 'banner-3'},
                {url: '@/assets/img/banner-4.jpg', alt: 'banner-4'},
                {url: '@/assets/img/banner-5.jpg', alt: 'banner-5'},
                {url: '@/assets/img/banner-6.jpg', alt: 'banner-6'},
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
            
        }
    }
}
</style>








<!-- <div class="col-2 logo-sposnor">
                    <img src="@/assets/img/banner-1.jpg" alt="">
                </div>
                <div class="col-2 logo-sposnor">
                    <img src="@/assets/img/banner-2.jpg" alt="">
                </div>
                <div class="col-2 logo-sposnor">
                    <img src="@/assets/img/banner-3.jpg" alt="">
                </div>
                <div class="col-2 logo-sposnor">
                    <img src="@/assets/img/banner-4.jpg" alt="">
                </div>
                <div class="col-2 logo-sposnor">
                    <img src="@/assets/img/banner-5.jpg" alt="">
                </div>
                <div class="col-2 logo-sposnor">
                    <img src="@/assets/img/banner-6.jpg" alt="">
                </div> -->