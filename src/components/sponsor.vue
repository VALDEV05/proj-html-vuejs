<template>
  <div id="background-sponsor"> 
      <div class="container">
            <div id="text-sponsor" class="text-center">
                <div class="title-sponsor text-uppercase fw-bold">
                    {{title}}
                </div>
                <div class="subtitle-sponsor pt-3">
                    {{subtitle}}
                </div>
            </div>
            <div class="row mt-4 py-3">
                <div class="col-2 logo-sponsor" v-for="banner in items" :key="banner.url">
                    <a href="#"><img :src="require('@/assets/img/' + banner.url)" :alt="banner.alt"></a>
                </div>
            </div>
      
      </div>
      
  </div>
</template>

<script>
export default {
    props:{
        title:String,
        subtitle:String,
        items:Array
    },

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