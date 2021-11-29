<template>
    <div class="container-jumbo text-center text-uppercase pt-3">
        <div class="title text-light">
            <p  class="m-0 title-sm">{{title}}</p>
            <p class="m-0 title-lg fw-bold">{{titleLG}}</p>
        </div> 
        <img src="@/assets/img/1-item-2.jpg" alt="">
        <div id="info" class="d-flex flex-row justify-content-center">
            <ul class="list-unstyled list-inline">
                <li class="px-3 list-inline-item" v-for="item in items" :key="item.data"><a class="text-light fw-bold text-uppercase text-decoration-none" href="#">{{item.info}}</a></li>
            </ul>
        </div>
        <div class="register">
            <button type="button" class="btn btn_register text-uppercase">{{buttonText}}</button>
        </div>
    </div>
</template>

<script>
export default {
props:{
    title:String,
    titleLG:String,
    buttonText:String,
    items:Array
},
}
</script>

<style lang="scss">
@import '@/assets/style/variables.scss';

#jumbotron_socialNetwork {
    background-image: url('../assets/img/slider-1-bg.jpg');
    width: 100vw;
    height: 500px;
    background-size: cover;
    background-repeat: no-repeat;
    background-position-y: center;
    .container-jumbo {
        height: 50%;
        .title-sm {
            font-size: 50px;
        }
        .title-lg {
            font-size: 90px;
            margin-top: -16px;
        }
        .btn_register {
            margin-top: 30px !important;
            background-color: $scarlet-red-color;
            color: $white-color;
            padding: 15px 40px;
        }
    }
}

</style>
