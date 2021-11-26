<template>
  <div id="jumbotron">
      <div class="container-jumbo pt-5">
          <h1 class="text-uppercase text-center fw-bold text-light pb-5">Tickets</h1>
          <div id="tickets" class="row d-flex justify-content-center gx-0">
              <div class="col ticket m-3">
                  <div class="headerTicket d-flex flex-column align-items-center">
                      <div class="titleTicket text-center pt-4">
                          <p class="m-0 fw-bold text-uppercase">One Day Pass</p>
                      </div>
                      <div class="priceTicket">
                          <p class="m-0 fw-bold text-uppercase">free</p>
                      </div>
                  </div>
                  <!-- /headerTicket -->
                  <div class="mainTicket d-flex align-items-center justify-content-center">
                      <ul class="list-unstyled text-center text-capitalized">
                            <li class="py-2">One Day Access</li>
                            <li class="py-2">Coffee Break</li>
                            <li class="py-2">Lunch (International Buffet)</li>
                            <li class="py-2">Document Sheets</li>
                            <li class="py-2">50USD Voucher For Next Event</li>
                      </ul>
                  </div>
                  <div class="footerTicket">
                      <p class="text-center text-uppercase text-light fw-bold"><a class="text-light text-decoration-none" href="#">Book now</a></p>
                  </div>
                  <!-- /footerTicket -->
              </div>
              <!-- /ticket -->
              <div class="col ticket m-3">
                  <div class="headerTicket d-flex flex-column align-items-center">
                      <div class="titleTicket text-center pt-4">
                          <p class="m-0 fw-bold text-uppercase">Four Day Pass</p>
                      </div>
                      <div class="priceTicket">
                          <p class="m-0 fw-bold text-uppercase">750.00 usd</p>
                      </div>
                  </div>
                  <!-- /headerTicket -->
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
                  <!-- /footerTicket -->
              </div>
              <!-- /ticket -->
              <div class="col ticket m-3">
                  <div class="headerTicket d-flex flex-column align-items-center">
                      <div class="titleTicket text-center pt-4">
                          <p class="m-0 fw-bold text-uppercase">Two Day Passes</p>
                      </div>
                      <div class="priceTicket">
                          <p class="m-0 fw-bold text-uppercase">580.00 usd</p>
                      </div>
                  </div>
                  <!-- /headerTicket -->
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
                  <!-- /footerTicket -->
              </div>
              <!-- /ticket -->

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
#jumbotron {
    background-image: url('../assets/img/ticket-bg.jpg');
    width: 100vw;
    height: 650px;
    background-size: contain;
    background-position: center;
    .container-jumbo {
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