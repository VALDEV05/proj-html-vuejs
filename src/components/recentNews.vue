<template>
  <div class="container">
        <div class="header row mt-5">
            <div class="col-4">
                <h1 class="text-uppercase fw-bold">Recent News</h1>
            </div>
            <div class="col"></div>
            <div class="col-2 text-end viewFull"><a href="#" class="text-decoration-none text-capitalized"> Read All News</a></div>
        </div>
        <div id="recentNewsCard" class="mt-5">
            <div class="row">
                <div class="col-4 d-flex justify-content-center">
                    <div class="card border-0" style="width: 26rem;">
                        <img src="@/assets/img/photodune-7770665-two-white-coffee-mug-with-diy-decoration-o (2).jpg" class="card-img-top" alt="...">
                        <div class="card-body">
                            <p class="sub-title m-0 pt-3 pb-2">03 Dec 2013 / 0 Comments</p>
                            <h5 class="card-title text-uppercase fw-bold pb-3">Sedial eiusmod tempor</h5>
                            <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente minima, excepturi officiis praesentium harum sunt neque explicabo ipsam odio sit? </p>
                            <p class="link"><a href="#" class="">Read More</a></p>
                        </div>
                    </div>
                </div>
                <div class="col-4 d-flex justify-content-center">
                    <div class="card border-0" style="width: 26rem;">
                        <img src="@/assets/img/photodune-8797753-multiethnic-people-with-startup-business-t (2).jpg" class="card-img-top" alt="...">
                        <div class="card-body">
                            <p class="sub-title m-0 pt-3 pb-2">03 Dec 2013 / 0 Comments</p>
                            <h5 class="card-title text-uppercase fw-bold pb-3">Donec luctus imperdiet</h5>
                            <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente minima, excepturi officiis praesentium harum sunt neque explicabo ipsam odio sit? </p>
                            <p class="link"><a href="#" class="">Read More</a></p>
                        </div>
                    </div>
                </div>
                <div class="col-4 d-flex justify-content-center">
                    <div class="card border-0" style="width: 26rem;">
                        <img src="@/assets/img/photodune-8522811-speaker-at-business-conference-and-present (2).jpg" class="card-img-top" alt="...">
                        <div class="card-body">
                            <p class="sub-title m-0 pt-3 pb-2">03 Dec 2013 / 0 Comments</p>
                            <h5 class="card-title text-uppercase fw-bold pb-3">magna pars studiorum</h5>
                            <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente minima, excepturi officiis praesentium harum sunt neque explicabo ipsam odio sit? </p>
                            <p class="link"><a href="#" class="">Read More</a></p>
                        </div>
                    </div>
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
.card{
    .sub-title{
        /* font-style: italic; */
        font-family: 'Bitter', serif;
        color: $icon-gray !important;
    }
    .card-text{
        color: $icon-gray !important;
    }
    .link a{
        color: $scarlet-red-color !important;
        text-decoration: none;
        font-family: 'Bitter', serif;
        &:hover{
            border-bottom: 1px solid $scarlet-red-color;
            cursor: pointer;
        }
    }
}
</style>
