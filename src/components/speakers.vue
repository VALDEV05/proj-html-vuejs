<template>
  <div class="container">
            <div class="controls d-flex justify-content-between">
                <div class="title_control">
                    <h1 class="text-uppercase fw-bold">{{title}}</h1>
                </div>
                <div class="controls_button d-flex">
                    <div class="btn_angle rounded-3 angle-left">&lt;</div>
                    <div class="btn_angle rounded-3 angle-right">&gt;</div>
                </div>
            <!-- /button controls -->
            </div>
            <!-- /controls -->
            <div class="section_card_speakers">
                <div class="row speaker">
                    <div class="col-3 container_card" v-for="card in items" :key="card.name">
                        <div class="card border-0" style="width: 18rem;">
                            <img :src="require('@/assets/img/' + card.image)" class="card-img-top image" alt="speaker-6">
                            <div class="text_card text-center pt-3">
                                <p class="m-0 title-card text-uppercase">{{card.name}}</p>
                                <p class="m-0 subtitle-card">{{card.role}}</p>
                            </div>
                            <div class="middle">
                                <div class="text text-light d-flex">
                                    <div class="square mx-1">
                                        <a href="https://twitter.com/?lang=it"><img src="@/assets/img/twitter-brands-celest-white.svg"  alt=""></a>
                                        
                                    </div>
                                    <div class="square mx-1">
                                        <a href="https://www.facebook.com/"><img src="@/assets/img/facebook-f-brands-white.svg" class="facebook" alt=""></a>
                                         
                                    </div>
                                    <div class="square mx-1">
                                        <a href="https://www.linkedin.com/"><img src="@/assets/img/linkedin-in-brands-white.svg" alt=""></a>
                                         

                                    </div>
                                </div>
                            </div>
                        </div>
                        <!-- /card -->
                    </div>
                    <!-- /col-card -->
                </div>
            </div>
        </div>
</template>

<script>
export default {
    props:{
        title:String,
        items:Array
    },
    data(){
        return{
            
        }
    }
}
</script>
<style lang="scss">
@import '@/assets/style/variables.scss';

#speakers{
    background-color: #f6f6f6;
    height: 700px;
    .controls{
        padding-top: 75px;
        .btn_angle{
        background-color: $primary-color;   
        height: 30px;
        width: 30px;
        padding: 20px;
        margin: 5px;
        display: flex;
        align-items: center;
        justify-content: center;
        color: white;
        font-weight: bold;
    
        }
    }
    .card{
            background-color: transparent !important;
            .card-img, .card-img-top {
                border-radius: 10px !important;
            }
            .title-card{
                font-size: 30px;
                padding: 10px 0;
                }
            
            .subtitle-card{
                color: gray;
            }
        }
}
.row.speaker {
    margin-top: 100px;
}
.container_card {
  position: relative;
  width: 50%;
}

.container_card:hover .middle {
    opacity: 0.6;
}

.text {
  font-size: 16px;
  padding: 16px 32px;
}
.middle {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 209px;
    width: 18rem;
    opacity: 0.0;
    transition: .5s ease;
     position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -75%);
    text-align: center;
    background-color: $primary-color;
}
.square{
    height: 70px;
    width: 70px;
    display: flex;
    align-items: center;
    justify-content: center;
    a{
        height: 100%;
        width: 100%;
    }
    img{
        transform: scale(.8);
    }

    .facebook{
        height: 90%;
    }
}
</style>