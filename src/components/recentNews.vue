<template>
  <div class="container">
        <div class="header row mt-5">
            <div class="col-4">
                <h1 class="text-uppercase fw-bold">{{title}}</h1>
            </div>
            <div class="col"></div>
            <div class="col-2 text-end viewFull"><a href="#" class="text-decoration-none text-capitalized"> {{viewFull}}</a></div>
        </div>
        <div id="recentNewsCard" class="mt-5">
            <div class="row">
                <div class="col-4 d-flex justify-content-center" v-for="card in items" :key="card.index">
                    <div class="card border-0" style="width: 26rem;">
                        <img :src="require('@/assets/img/' + card.imageUrl)" class="imgNews" alt="">
                        <div class="card-body">
                            <p class="sub-title m-0 pt-3 pb-2">{{card.subtitle}}</p>
                            <h5 class="card-title text-uppercase fw-bold pb-3">{{card.title}}</h5>
                            <p class="card-text">{{card.text}}</p>
                            <p class="link"><a href="#" class="">{{card.linkText}}</a></p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
  </div>
</template>

<script>
export default {
    props:{
        title:String,
        viewFull:String,
        items:Array,
    },
}
</script>

<style lang="scss">
@import '@/assets/style/variables.scss';
.card{
    .sub-title{
        /* font-style: italic; */
        font-family: 'Bitter', serif;
        color: $icon-gray !important;
    }
    .card-text{
        color: $icon-gray !important;
    }
    .link a{
        color: $primary-color !important;
        text-decoration: none;
        font-family: 'Bitter', serif;
        &:hover{
            cursor: pointer;
            border-bottom: 1px solid $primary-color;
        }
    }
    .imgNews{
        &:hover{
            filter: brightness(80%);
            transition: filter .5s;
        }
    }
}
</style>
