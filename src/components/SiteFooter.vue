<template>
  <div id="siteFooter">
    <div class="main">
      <div class="container">
          <div class="row text-light">
            <div class="col-3 mt-5">
              <h1 class="text-uppercase">{{titleFirstCol}}</h1>
              <p class="paragraph">{{subtitleFirstCol}}</p>
              <div class="row social">
                <div class="col-2" v-for="icon in iconSocial" :key="icon.icon">
                  <div class="square d-flex justify-content-center align-items-center">
                    <a :href="icon.iconLink"><img :src="require('@/assets/img/' + icon.iconUrl)" alt=""></a>
                  </div>
                </div>

              </div>
            </div>
            <div class="col-3 mt-5">
              <h1 class="text-uppercase">{{titleSecondCol}}</h1>
              <div class="recentNews" v-for="news in recentNews" :key="news.news">
                  <p><a class="text-decoration-none text-light text-uppercase text-muted" href="#">&gt; &emsp14; {{news.news}}</a></p>
              </div>
              
            </div>
            <div class="col-3 mt-5" >
              <h1 class="text-uppercase">{{titleThirdCol}}</h1>
              <p>{{subtitleThirdCol}}</p>
              <div class="checkBtn mt-4 text-uppercase text-center fw-bold"><a href="#" class="text-light text-decoration-none">{{checkThirdCol}}</a> </div>
            </div>
            <div class="col-3 mt-5 gallery">
              <h1 class="text-uppercase">{{titleFourCol}}</h1>
              <div class="row text-opacity-50">
                <div class="col-3 m-0" v-for="img in gallery" :key="img.img">
                  <img :src="require('@/assets/img/' + img.imageUrl)" alt="">
                </div>
              </div>
            </div>
          </div>
      </div>
    </div> 
    <div class="footer">
      <div class="container d-flex justify-content-between align-items-center">
        <div class="row w-100" style="background-color:black">
          <div class="col-6 text-muted">
              <p>&copy; Copyright GoodLayers, All Right Reserverd</p>
          </div>
          <div class="col-6 text-muted text-end">
            <div class="right d-flex">
               <p>About Us| Accommodation | Call For Paper | Contact Us</p>
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
      titleFirstCol:'About us',
      subtitleFirstCol:'Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.',
      titleSecondCol:'Recent news',
      titleThirdCol:'get your seat!',
      subtitleThirdCol: "Book for your seat before it's too rate. we provide variety of ticket options",
      checkThirdCol:'check out tickets!',
      titleFourCol:'gallery from last year',
      iconSocial:[
        {
          iconUrl:'icon-square/facebook-square-brands.svg',
          iconLink:'https://www.facebook.com/'
        },
        {
          iconUrl:'icon-square/twitter-square-brands.svg',
          iconLink:'https://twitter.com/?lang=it'
        },
        {
          iconUrl:'icon-square/linkedin-brands.svg',
          iconLink:'https://www.linkedin.com/'
        },
        {
          iconUrl:'icon-square/google-plus-square-brands.svg',
          iconLink:'https://it.wikipedia.org/wiki/Google%2B/'
        },
        {
          iconUrl:'icon-square/pinterest-square-brands.svg',
          iconLink:'https://www.pinterest.it/'
        },
        {
          iconUrl:'icon-square/double-dot-square.svg',
          iconLink:'#'
        },

      ],
      recentNews:[
        {news:'Sem porta mollis parturient'},
        {news:'nullam lorem mattis purus'},
        {news:'nibm sem sit ullamcorporer'},
        {news:'donec luctus imperdiet'},
        {news:'magna pars studiorum'},
      ],
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
      links:[
        {link:'About Us |'},
        {link:'Accommodation |'},
        {link:'Call For Paper|'},
        {link:'Contact Us |'},

      ]
    }
  }
}
</script>

<style  lang="scss">
@import '@/assets/style/variables.scss';
#siteFooter{
  height: 467;
  .main{
    background-color: $background-footer;
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
        background-color: $primary-color;
        width: 65%;
        padding: 12px 10px;
      }
    }
    .gallery{
      margin-bottom: 40px;
    }
    .row.social{
      width: 85%;
    }
    .square{
      height: 35px;
      width: 35px;
      border-radius: 5px;
      img{
        filter: invert(1);
      }
    }
  }
  .footer{
    height: 100px;
    background-color: $black-color;
    .container{
      height: 100%;
      .right{
        margin-left: 195px;
      }
    }
  }
  
}

</style>