<template>
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
                subscribe for update
                <div id="input_countdown" class="mt-4 d-flex align-items-center justify-content-center">
                    <input type="text" id="input_countdown" class="py-1" >
                <button class="btn_subscribe py-3 fw-bold">subcribe</button>
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
                    box-shadow: 10px 10px 5px  $black-color;
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
            background: $primary-color;
            border: none;
            color: $white-color;
            text-transform: uppercase;
            box-shadow:  2px  rgb(78, 18, 18);
        }

}

</style>