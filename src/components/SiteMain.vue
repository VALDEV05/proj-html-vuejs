<template>
  <div id="siteMain"> 
      <div id="jumbotron_socialNetwork" class="d-flex align-items-center"> 
          <div class="container-jumbo text-center text-uppercase">
              <div class="title text-light">
                  <p  class="m-0 title-sm">Conference on</p>
                  <p class="m-0 title-lg fw-bold">social networks</p>
              </div> 
              <img src="@/assets/img/1-item-2.jpg" alt="">
              <div id="info" class="d-flex flex-row justify-content-center">
                  <ul class="list-unstyled list-inline">
                      <li class=" list-inline-item"><a class="text-light fw-bold text-uppercase text-decoration-none" href="#">23 - 26 MAY 2019 </a></li>
                      <li class="px-4 list-inline-item"><a class="text-light fw-bold text-uppercase text-decoration-none" href="#"> / </a></li>
                      <li class=" list-inline-item"><a class="text-light fw-bold text-uppercase text-decoration-none" href="#"> SANS FRANCISCO </a></li>
                      <li class="px-4 list-inline-item"><a class="text-light fw-bold text-uppercase text-decoration-none" href="#"> / </a></li>
                      <li class="list-inline-item"><a class="text-light fw-bold text-uppercase text-decoration-none" href="#"> 8 SPEAKERS </a></li>
                  </ul>
              </div>
              <div class="register">
                  <button type="button" class="btn btn_register text-uppercase">register online</button>
              </div>
          </div>
    
    
   
    </div>
    <div class="section_card container">
        <div class="row mt-5">
            <div class="col card_main d-flex">
                <img src="../assets/img/trophy-solid.svg" alt="trophy">
                <div id="text_card" class="mx-4">
                    <p class="title_card text-uppercase">Who we are</p>
                    <p class="text-muted">Donec id elit non mi porta gravida at eget me tus. Sed posuere consectutyr estat lobo rtis. Cum sociis natoque.</p>
                    <p><a href="#" class="learn_more_font">Learn More</a></p>
                </div>
            </div>
            <div class="col card_main d-flex">
                <img src="../assets/img/bolt-solid.svg" alt="bolt">
                <div id="text_card" class="mx-4">
                    <p class="title_card text-uppercase">Who we are</p>
                    <p class="text-muted">Donec id elit non mi porta gravida at eget me tus. Sed posuere consectutyr estat lobo rtis. Cum sociis natoque.</p>
                    <p><a href="#" class="learn_more_font">Learn More</a></p>
                </div>

            </div>
            <div class="col card_main d-flex">
                <img src="../assets/img/question-solid.svg" alt="question">
                <div id="text_card" class="mx-4">
                    <p class="title_card text-uppercase">Who we are</p>
                    <p class="text-muted">Donec id elit non mi porta gravida at eget me tus. Sed posuere consectutyr estat lobo rtis. Cum sociis natoque.</p>
                    <p><a href="#" class="text-decoration-none learn_more_font">Learn More</a></p>
                </div>
            </div>
        </div>
    </div>
    <div id="jumbotron_countdown" class="jumbotronClass mt-5">
        <div class="container-jumbo">
            <div class="row pt-5">
                <div class="col-3 countdown d-flex justify-content-center align-items-center">
                    <div class="square d-flex flex-column align-items-center justify-content-center">
                        <p id="number" class="m-0">
                             3399  
                        </p>
                        <p class="text_countodown text-uppercase">days</p>
                    </div>
                </div>
                <div class="col-3 countdown d-flex justify-content-center align-items-center">
                    <div class="square d-flex flex-column align-items-center justify-content-center">
                        <p id="number" class="m-0">
                             17   
                        </p>
                        <p class="text_countodown text-uppercase">hours</p>
                    </div>
                </div>
                <div class="col-3 countdown d-flex justify-content-center align-items-center">
                    <div class="square d-flex flex-column align-items-center justify-content-center">
                        <p id="number" class="m-0">
                             28   
                        </p>
                        <p class="text_countodown text-uppercase">mins</p>
                    </div>
                </div>
                <div class="col-3 countdown d-flex justify-content-center align-items-center">
                    <div class="square d-flex flex-column align-items-center justify-content-center">
                        <p id="number" class="m-0">
                             17   
                        </p>
                        <p class="text_countodown text-uppercase">secs</p>
                    </div>
                </div>

            </div>
            <div id="text_jumbo_countdown" class="text-uppercase fw-bold" >
                subscribe for updatae
                <div id="input_countdown" class="mt-4 d-flex align-items-center justify-content-center   ">
                    <input type="text" id="input_countdown">
                <button class="btn_subscribe">subcribe</button>
                </div>
                
            </div>
        </div>
    </div>
  </div>
  <!-- /siteMain -->
</template>

<script>
export default {
    props:{
        title:String,
    }
}
</script>

<style  lang="scss">
@import '@/assets/style/variables.scss';
#jumbotron_socialNetwork {
    background-image: url('../assets/img/slider-1-bg.jpg');
    width: 100vw;
    height: 700px;
    background-size: cover;
    background-repeat: no-repeat;
    background-position-y: center;
    .container-jumbo {
        height: 50%;
        .title-sm {
            font-size: 50px;
        }
        .title-lg {
            font-size: 90px;
            margin-top: -16px;
        }
        .btn_register {
            margin-top: 30px !important;
            background-color: $scarlet-red-color;
            color: $white-color;
            padding: 15px 40px;
        }
    }
}
.section_card {
    .card_main {
        width: 33.33%;
        img {
            height: 50px;
            width: 50px;
            color: $icon-gray;
        }
        #text_card {
            .title_card {
                font-size: 25px;
                font-weight: bold;
            }
            p a {
                text-decoration: none;
                color: $scarlet-red-color;
                font-family: 'Bitter', serif;
            }
        }
    }
}

#jumbotron_countdown {
    background-image: url('../assets/img/coutdown-bg1.jpg');
    width: 100vw;
    height: 500px;
    background-size: cover;
    background-repeat: no-repeat;
    background-position-y: center;
    .container-jumbo{
        height: 100%;
        .countdown{
            height: 200px;
            color: $white-color;
            .square{
                height: 170px;
                width: 220px;
                background-color: rgba($black-color, $alpha: 0.5);
                border-radius: 15px;
                font-weight: 700;
                #number{
                    font-size: 80px;
                }
                .text_countodown{
                    font-size: 30px;
                }
                &:hover{
                    background-color: rgba($black-color, $alpha: 0.8);
                    box-shadow: 10px 10px 5px  black;
                    height: 190px;
                    width: 250px;   
                    transition: height 4s, width 2s;
                }
            } 
        }
        #text_jumbo_countdown{
            font-size: 40px;
            text-align: center;
            margin-top: 20px;}
        }
        .btn_subscribe {
            font-size: 24px;
            margin-left: 15px;
            padding: 15px 20px;
            background: red;
            border: none;
            color: white;
            text-transform: uppercase;
        }

}
</style>