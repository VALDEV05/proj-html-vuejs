<template>
    <div id="location_jumbo">
        <div class="container-jumbo text-center pt-3" v-for="item in items" :key="item.item">
            <div class="title text-light">
                <p  class="m-0 title-lg py-5 text-uppercase">{{item.title}}</p>
                <p class="m-0 title-sm text-uppercase">{{item.subtitle}}</p>
                <div id="address" class="d-flex justify-content-center mt-3">
                    <img :src="require('@/assets/img/' + item.address.icon)" :alt="item.address.alt" style="height:20px; width:20px;" class="me-3">
                    <p>{{item.address.text}}</p> 
                </div>
                <p class="m-3 check"><a href="#" class="text-capitalize">{{item.check}}</a></p>
            </div> 
            <img src="@/assets/img/1-item-2.jpg" alt="">
            <div id="info" class="d-flex flex-row justify-content-center">
                <ul class="list-unstyled list-inline">
                    <li class="me-3 list-inline-item"><a class="text-light text-decoration-none" href="#"><img :src="require('@/assets/img/' + item.contacts.phone.icon)" :alt="item.contacts.phone.alt" style="height:20px; width:20px;"> <span class="ms-2"> {{item.contacts.phone.number}}</span></a></li>
                    <li class=" ms-3 list-inline-item"><a class="text-light text-decoration-none" href="#"> <img :src="require('@/assets/img/' + item.contacts.email.icon)" style="height:20px; width:20px;" :alt="item.contacts.email.alt"> <span class="ms-2"> {{item.contacts.email.address}}</span></a></li>
                </ul>
            </div>
        </div>
  </div>
  <!-- /#location_jumbo -->
</template>
<script>
export default {
    props:{
        items:Array
    }
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
            color: $primary-color;
            text-decoration: none;
            &:hover{
                cursor: pointer;
                /* text-decoration: underline; */
                border-bottom: 1px solid $primary-color;
            }
        }
    }
}

</style>