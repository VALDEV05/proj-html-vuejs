<template>
  <div class="container">
      <div class="header row mt-5">
            <div class="col-3">
                <h1 class="text-uppercase fw-bold">Program</h1>
            </div>
            <div class="col text-start">
                <p class="text-muted">This conference run through all 4 days from 23-26 May 2016,<br>
                            We also provide free lunch and coffee break in each day
                </p>
            </div>
            <div class="col-2 text-end viewFull"><a href="#" class="text-decoration-none"> View Full Program</a></div>
      </div>
      <!-- /header -->
      <div id="timeline" class="mt-5">
          <div class="row">
              <div class="col-2 day ps-4 py-3">
                  <h1 class="m-0 py-2">Day 1</h1>
                  <p class="m-0">23 May 2016</p>
              </div>
              <div class="col-2 day ps-4 py-3">
                  <h1 class="m-0 py-2">Day 2</h1>
                  <p class="m-0">24 May 2016</p>
              </div>
              <div class="col-2 day ps-4 py-3">
                  <h1 class="m-0 py-2">Day 3</h1>
                  <p class="m-0">25 May 2016</p>
              </div>
              <div class="col-2 day ps-4 py-3">
                  <h1 class="m-0 py-2">Day 4</h1>
                  <p class="m-0">26 May 2016</p>
              </div>
              <div class="col-2 day ps-4 py-3">
                  <h1 class="m-0 py-2">Day 5</h1>
                  <p class="m-0">27 May 2016</p>
              </div>
              <div class="col-2 day ps-4 py-4">
              </div>
          </div>
      </div>
      <!-- /timeline -->
      <div id="section_days" class="row pt-5">
          <div class="col-3 info d-flex align-items-center">
              <div id="data_section_info" >
                  <div id="clock" class="d-flex py-2">
                    <img src="@/assets/img/clock-regular.svg" style="height: 25px; width: 25px;" alt="clock">
                    <p class="ms-4 m-0 text-muted text-uppercase">09:00-10:30</p>  
                  </div>
                  <div id="location" class="d-flex py-2">
                    <img src="@/assets/img/location-arrow-solid.svg" style="height: 25px; width: 25px;" alt="clock">
                    <p class="ms-4 m-0 text-muted text-uppercase">room A</p>  
                  </div>
                  <div id="user" class="d-flex py-2">
                    <img src="@/assets/img/user-solid.svg" style="height: 25px; width: 25px;" alt="clock">
                    <p class="ms-4 m-0 text-muted text-uppercase">Laurence francis</p>  
                  </div>
                  
              </div>
          </div>
          <div class="col-9 mb-4">
              <div id="text_section_info">
                  <h1 class="text-uppercase mt-4"> Welcoming and introduction</h1>
                  <p class="py-4">Vestibulum id ligula porta felis euismod semper. Nullam quis risus eget urna mollis ornare vel eu leo. Donec ullamcorper nella non metus auctor fringilla. Aenean lacinia bibendu, nulla sed cosectetur...</p>
                  <img src="@/assets/img/speaker-8.jpg" style="height: 80px; width: 100px;" class="rounded-3" alt="speaker-8">
              </div>
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
.viewFull a{
    font-style: italic;
    font-family: 'Bitter', serif;
    color: $scarlet-red-color !important;
}
.day{
    background-color: $scarlet-red-color;
    border-left: 1px solid $black-color;
    color: $white-color;
    h1{
        margin: 20px 0px;
        font-weight: bold;
        font-size: 25px;
    }
}
#section_days{
    background-color: #F3F3F3;
    .user{
        p{

        }
    }
    .info{
        height: 200px;
        #data_section_info{
            height: 150px;
            width: 200px;
            margin: auto;

        }
    }
}
</style>