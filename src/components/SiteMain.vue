<template>
  <div id="siteMain"> 
      <div id="jumbotron_socialNetwork" class="d-flex align-items-center"> 
          <div class="container text-center text-uppercase">
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
    <div id="jumbotron_countdown" class="jumbotronClass mt-5"></div>
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

</style>