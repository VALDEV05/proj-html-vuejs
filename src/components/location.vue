<template>
    <div id="location_jumbo">
        <div class="container-jumbo text-center pt-3">
            <div class="title text-light">
                <p  class="m-0 title-lg py-5 text-uppercase">Location</p>
                <p class="m-0 title-sm text-uppercase">Gd building, grand conference room</p>
                <div id="address" class="d-flex justify-content-center mt-3">
                    <img src="@/assets/img/location-arrow-solid-white.svg" style="height:20px; width:20px;" class="me-3" alt="location">
                    <p>11 GD Building, River Mail, New York, USA 8879</p> 
                </div>
                <p class="m-3 check"><a href="#" class="text-capitalize">Check For accomodations here</a></p>
            </div> 
            <img src="@/assets/img/1-item-2.jpg" alt="">
            <div id="info" class="d-flex flex-row justify-content-center">
                <ul class="list-unstyled list-inline">
                    <li class="me-3 list-inline-item"><a class="text-light text-decoration-none" href="#"><img src="@/assets/img/phone-alt-solid-white.svg" style="height:20px; width:20px;"  alt=""> <span class="ms-2"> +1-112-222-3344</span></a></li>
                    <li class=" ms-3 list-inline-item"><a class="text-light text-decoration-none" href="#"> <img src="@/assets/img/envelope-solid-white.svg" style="height:20px; width:20px;"  alt=""> <span class="ms-2"> Contact@TheKeynoteTheme.com</span></a></li>
                </ul>
            </div>
        </div>
  </div>
  <!-- /#location_jumbo -->
</template>
<script>
export default {

}
</script>

<style lang="scss">
@import '@/assets/style/variables.scss';

#location_jumbo{
    background-image: url('../assets/img/location-bg.jpg');
    width: 100vw;
    height: 500px;
    background-size: cover;
    background-repeat: no-repeat;
    background-position-y: center;
    .container-jumbo {
        height: 50%;
        .title-sm {
            font-size: 35px;
        }
        .title-lg {
            font-size: 60px;
            margin-top: -16px;
        }
        .check a{
            color: $scarlet-red-color;
            text-decoration: none;
            &:hover{
                cursor: pointer;
                /* text-decoration: underline; */
                border-bottom: 1px solid $scarlet-red-color;
            }
        }
    }
}

</style>