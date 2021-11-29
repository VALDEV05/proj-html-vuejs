<template>
  <div class="container">
      <div class="header row mt-5">
            <div class="col-3">
                <h1 class="text-uppercase fw-bold">{{title}}</h1>
            </div>
            <div class="col text-start">
                <p class="text-muted">{{subtitle}}</p>
            </div>
            <div class="col-2 text-end viewFull"><a href="#" class="text-decoration-none"> View Full Program</a></div>
      </div>
      <!-- /header -->
      <div id="timeline" class="mt-5">
          <div class="row">
              <div class="col-2 day ps-4 py-3" v-for="(day, index) in days" :key="index">
                  <h1 class="m-0 py-2">{{day.day}}</h1>
                  <p class="m-0">{{day.date}}</p>
              </div>
          </div>
      </div>
      <!-- /timeline -->
      <div id="section_days" class="row pt-5" v-for="item in items" :key="item.item">
          <div class="col-3 info d-flex align-items-center">
              <div id="data_section_info" >
                  <div id="clock" class="d-flex py-2">
                    <img :src="require('@/assets/img/' + item.firstDay.hour.icon)" style="height: 25px; width: 25px;" alt="clock">
                    <p class="ms-4 m-0 text-muted text-uppercase">{{item.firstDay.hour.hourly}}</p>  
                  </div>
                  <div id="location" class="d-flex py-2">
                    <img :src="require('@/assets/img/' + item.firstDay.location.icon)" style="height: 25px; width: 25px;" alt="clock">
                    <p class="ms-4 m-0 text-muted text-uppercase">{{item.firstDay.location.room}}</p>  
                  </div>
                  <div id="user" class="d-flex py-2">
                    <img :src="require('@/assets/img/' + item.firstDay.speaker.icon)" style="height: 25px; width: 25px;" alt="clock">
                    <p class="ms-4 m-0 text-muted text-uppercase">{{item.firstDay.speaker.name}}</p>  
                  </div>
                  
              </div>
          </div>
          <div class="col-9">
              <div id="text_section_info">
                  <h1 class="text-uppercase mt-4"> {{item.firstDay.program.title}}</h1>
                  <p class="py-4">{{item.firstDay.program.subtitle}}</p>
                  <img class="speaker" :src="require('@/assets/img/' + item.firstDay.speaker.image)" style="height: 80px; width: 100px;" alt="speaker-8">
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
        days:Array,
        items:Array
    },
}
</script>

<style lang="scss">
@import '@/assets/style/variables.scss';
.viewFull a{
    font-style: italic;
    font-family: 'Bitter', serif;
    color: $primary-color !important;
}
.day{
    background-color: $primary-color;
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
    .info{
        height: 200px;
        #data_section_info{
            height: 150px;
            width: 200px;
            margin: auto;

        }
    }
}
.speaker{
    margin-bottom: 150px;
    border-radius: 10px;
}
</style>