<template>
  <div id="siteFooter">
      <div class="container">
        <div class="row text-light">
          <div class="col-3 mt-5">
            <h1 class="text-uppercase">about us</h1>
            <p class="paragraph">Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.</p>
            <div class="row social">
              <div class="col-2">
                <div class="square">
                  <a href="#"></a>
                </div>
              </div>
              <div class="col-2">
                <div class="square"></div>
              </div>
              <div class="col-2">
                <div class="square"></div>
              </div>
              <div class="col-2">
                <div class="square"></div>
              </div>
              <div class="col-2">
                <div class="square"></div>
              </div>
              <div class="col-2">
                <div class="square"></div>
              </div>

            </div>
          </div>
          <div class="col-3 mt-5">
            <h1 class="text-uppercase">Recent news</h1>
            <p><a class="text-decoration-none text-light text-uppercase" href="#">&gt; &emsp14; Sem porta mollis parturient</a></p>
            <p><a class="text-decoration-none text-light text-uppercase" href="#">&gt; &emsp14; Sem porta mollis parturient</a></p>
            <p><a class="text-decoration-none text-light text-uppercase" href="#">&gt; &emsp14; Sem porta mollis parturient</a></p>
            <p><a class="text-decoration-none text-light text-uppercase" href="#">&gt; &emsp14; Sem porta mollis parturient</a></p>
            <p><a class="text-decoration-none text-light text-uppercase" href="#">&gt; &emsp14; Sem porta mollis parturient</a></p>
          </div>
          <div class="col-3 mt-5" >
            <h1 class="text-uppercase">get your seat!</h1>
            <p>Book for your seat before it's too rate. we provide variety of ticket options</p>
            <div class="checkBtn mt-4 text-uppercase text-center fw-bold"><a href="#" class="text-light text-decoration-none">check out tickets!</a> </div>
          </div>
          <div class="col-3 mt-5 gallery">
            <h1 class="text-uppercase">{{titleGallery}}</h1>
            <div class="row">
              <div class="col-3 m-0" v-for="img in gallery" :key="img.img">
                <img :src="require('@/assets/img/' + img.imageUrl)" alt="">
              </div>
            </div>
          </div>
          
        </div>  
      </div>
  </div>
  <!-- /siteFooter -->
</template>

<script>
export default {

  data(){
    return{
      titleGallery:'gallery from last year',
      gallery:[
        {imageUrl:'photodune-7770665-two-white-coffee-mug-with-diy-decoration-o (1).jpg'},
        {imageUrl:'photodune-8523683-speaker-at-business-convention-and-present.jpg'},
        {imageUrl:'photodune-6745579-modern-creative-man-relaxing-on-workspace-.jpg'},
        {imageUrl: 'photodune-8522811-speaker-at-business-conference-and-present (1).jpg'},
        {imageUrl:'photodune-8797753-multiethnic-people-with-startup-business-t.jpg'},
        {imageUrl:'card04-150x150.jpg'},
        {imageUrl:'photodune-6745606-man-wristwatch-calendar-key-and-glasses-on.jpg'},
        {imageUrl:'photodune-6745585-modern-creative-workspace-m-150x150.jpg'},
        {imageUrl:'6426608875_186070f8ca_o-150x150.jpg'},
        {imageUrl:'card01-150x150.jpg'},
        {imageUrl:'13349065283_64d09b067c_o-150x150.jpg'},
        {imageUrl:'photodune-8795110-overhead-of-essentials-denim-clothes-m.jpg'}],

    }
  }
}
</script>

<style  lang="scss">
@import '@/assets/style/variables.scss';
#siteFooter{
  background-color: $background-footer;
  height: 400px;
  h1{
    font-size: 20px;
    margin-bottom: 30px;
  }
  .col-3 > img{
    margin-top: 15px;
    height: 60px;
    width: 60px;
  }
  .col-3{
    .paragraph{
      width: 85%;

    }
    .checkBtn{
      background-color: $scarlet-red-color;
      width: 65%;
      padding: 12px 10px;
    }
  }
  .row.social{
    width: 85%;
  }
  .square{
    background-color: white;
    height: 35px;
    width: 35px;
    border-radius: 5px;
  }
}

</style>