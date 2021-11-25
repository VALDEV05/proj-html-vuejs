<template>
  <div id="siteMain"> 
      <div id="jumbotron" class="d-flex align-items-center"> 
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
                  <button type="button" class="mt-4 btn btn_register text-uppercase">register online</button>
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

</style>