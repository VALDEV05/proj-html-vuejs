<template>
  <div class="container">
      <div class="row">
          <div class="col-6 video my-4">
          <h1 class="text-uppercase">Presentation</h1>
          <img src="@/assets/img/presentation-control-bar.svg" alt="pres-control">
          </div>
      <div class="col-6 my-4">
          <h1 class="text-uppercase">twitter feed</h1>
          <ul class="list-unstyled">
              <li class="tweet mb-4 d-flex">
                  <img src="@/assets/img/twitter-brands-celest.svg" style="height:50px; width:50px;" alt="">
                  <div id="text_message" class="ms-4">
                      <div class="text_message">
                        Stand out and be vibrant with some of the best bright and bold templates on <span>@Envato</span> Elements. And add a splash of c... <span>https://t.co/jFrsnzEJK7</span>
                      </div>
                      <div class="date mt-4">
                          3 days ago
                      </div>
                  </div>
              </li>
              <li class="tweet mb-4 d-flex">
                  <img src="@/assets/img/twitter-brands-celest.svg" style="height:50px; width:50px;" alt="">
                  <div id="text_message" class="ms-4">
                      <div class="text_message">
                        Stand out and be vibrant with some of the best bright and bold templates on <span>@Envato</span> Elements. And add a splash of c... <span>https://t.co/jFrsnzEJK7</span>
                      </div>
                      <div class="date mt-4">
                          9 days ago
                      </div>
                  </div>
              </li>
              <li class="tweet mb-4 d-flex">
                  <img src="@/assets/img/twitter-brands-celest.svg" style="height:50px; width:50px;" alt="">
                  <div id="text_message" class="ms-4">
                      <div class="text_message">
                        Stand out and be vibrant with some of the best bright and bold templates on <span>@Envato</span> Elements. And add a splash of c... <span>https://t.co/jFrsnzEJK7</span>
                      </div>
                      <div class="date mt-4">
                          11 days ago
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