<template>
  <div id="jumbotron">
      <div class="container pt-5">
          <h1 class="text-uppercase text-center fw-bold text-light pb-3">{{title}}</h1>
          <div id="tickets" class="row d-flex justify-content-center gx-0">
              <div class="col ticket m-3" v-for="ticket in items" :key="ticket.ticket">
                  <div class="headerTicket d-flex flex-column align-items-center">
                      <div class="titleTicket text-center pt-4">
                          <p class="m-0 fw-bold text-uppercase">{{ticket.durationTicket}}</p>
                      </div>
                      <div class="priceTicket">
                          <p class="m-0 fw-bold text-uppercase">{{ticket.priceTicket}}</p>
                      </div>
                  </div>
                  <!-- /headerTicket -->
                    <div class="mainTicket d-flex align-items-center justify-content-center">
                      <ul class="list-unstyled text-center text-capitalized">
                            <li class="py-2">{{ticket.included.duration}}</li>
                            <li class="py-2">{{ticket.included.beverage}}</li>
                            <li class="py-2">{{ticket.included.food}}</li>
                            <li class="py-2">{{ticket.included.documentation}}</li>
                            <li class="py-2">{{ticket.included.bonus}}</li>
                      </ul>
                    </div>
                
                  <div class="footerTicket">
                      <p class="text-center text-uppercase text-light fw-bold"><a class="text-light text-decoration-none" href="#">{{button}}</a></p>
                  </div>
                  <!-- /footerTicket -->
              </div>
              <!-- /ticket -->
              <!-- <div class="col ticket m-3">
                  <div class="headerTicket d-flex flex-column align-items-center discount">
                      <div class="titleTicket text-center pt-4">
                          <p class="m-0 fw-bold text-uppercase">Four Day Pass</p>
                      </div>
                      <div class="priceTicket">
                          <p class="m-0 fw-bold text-uppercase">750.00 usd</p>
                      </div>
                  </div>
                  <div class="mainTicket d-flex align-items-center justify-content-center">
                      <ul class="list-unstyled text-center text-capitalized">
                            <li class="py-2">Four Day Access</li>
                            <li class="py-2">Coffee Break</li>
                            <li class="py-2">Lunch (International Buffet)</li>
                            <li class="py-2">Document Sheets</li>
                            <li class="py-2">100USD Voucher For Next Event</li>
                      </ul>
                  </div>
                  <div class="footerTicket">
                      <p class="text-center text-uppercase text-light fw-bold"><a class="text-light text-decoration-none" href="#">Book now</a></p>
                  </div>
              </div>

              <div class="col ticket m-3">
                  <div class="headerTicket d-flex flex-column align-items-center">
                      <div class="titleTicket text-center pt-4">
                          <p class="m-0 fw-bold text-uppercase">Two Day Passes</p>
                      </div>
                      <div class="priceTicket">
                          <p class="m-0 fw-bold text-uppercase">580.00 usd</p>
                      </div>
                  </div>
                  <div class="mainTicket d-flex align-items-center justify-content-center">
                      <ul class="list-unstyled text-center text-capitalized">
                            <li class="py-2">Two Day Access</li>
                            <li class="py-2">Coffee Break</li>
                            <li class="py-2">Lunch (International Buffet)</li>
                            <li class="py-2">Document Sheets</li>
                            <li class="py-2">70USD Voucher For Next Event</li>
                      </ul>
                  </div>
                  <div class="footerTicket">
                      <p class="text-center text-uppercase text-light fw-bold"><a class="text-light text-decoration-none" href="#">Book now</a></p>
                  </div> 
              </div>-->


          </div>
      </div>
  </div>
</template>

<script>
export default {
props:{
    title:String,
    items:Array,
    button:String
},
}
</script>

<style lang="scss">
@import '@/assets/style/variables.scss';
#jumbotron {
    background-image: url('../assets/img/ticket-bg.jpg');
    width: 100vw;
    height: 595px;
    background-size: contain;
    background-position: center;
    .container {
        .ticket{
            height: 400px;
            background-color: #F9F9F9;
            .headerTicket{
                height: 90px;
                background-color: #E9E9E9; 
                .priceTicket{
                    p{
                        color: $scarlet-red-color;
                    }
                }
            }
            .mainTicket{
                height: calc(400px - 160px);
                font-family: 'Bitter', serif;
                color: $icon-gray !important;
                li{
                    font-size: 15px;
                }
            }
            .footerTicket{
                height: 70px;
                background-color: $scarlet-red-color;
                line-height: 70px;
                vertical-align: middle;
                p a:hover{
                    border-bottom:px solid white;
                    cursor: pointer;
                }
                

            }
        }   
    }
}
</style>