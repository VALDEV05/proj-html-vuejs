<template>
  <div class="container row">
      <div class="col-6 video my-4">
          <h1 class="text-uppercase">Presentation</h1>
          <div class="video">
            <img src="@/assets/img/461365506.webp" alt="">
            <div class="control-bar">
                <img src="@/assets/img/bar-control-video.svg" alt="">
            </div>
          </div>
         
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
</template>

<script>
export default {

}
</script>

<style lang="scss">
@import '@/assets/style/variables.scss';

.col-6.video{
    display: flex;
    flex-direction: column;
    .video{
        position: relative;
        img{
            margin-left: 70px;
        }
    }
    .control-bar{
        position: absolute;
        bottom: 0px;
        right: 10px;
        img{
            width: 550px;
        }
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