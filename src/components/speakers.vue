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
                <div class="row mt-5">
                    <div class="col-3 container_card" v-for="card in cards" :key="card.name">
                        <div class="card border-0" style="width: 18rem;">
                            <img :src="require('@/assets/img/' + card.image)" class="card-img-top image" alt="speaker-6">
                            <div class="text_card text-center pt-3">
                                <p class="m-0 title-card text-uppercase">{{card.name}}</p>
                                <p class="m-0 subtitle-card">{{card.role}}</p>
                            </div>
                            <div class="middle">
                                <div class="text text-light d-flex">
                                    <div class="square mx-1">
                                        <img src="@/assets/img/twitter-brands-white.svg"  alt="">
                                    </div>
                                    <div class="square mx-1">
                                         <img src="@/assets/img/facebook-f-brands-white-h70.svg" alt="">
                                    </div>
                                    <div class="square mx-1">
                                         <img src="@/assets/img/linkedin-in-brands-white.svg" alt="">

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
    },
    data(){
        return{
            cards:[
                {   
                    image:'speaker-6.jpg',
                    alt:'speaker-6',
                    name:'patrick spencer',
                    role:'S&P Analyzer'
                },
                {   
                    image:'speaker-5.jpg',
                    alt:'speaker-5',
                    name:'janet jones',
                    role:" Newyork Post's GM"
                },
                {   
                    image:'speaker-4.jpg',
                    alt:'speaker-4',
                    name:'Michael dover',
                    role: "Starbuck's CEO"
                },
                {   
                    image:'speaker-3.jpg',
                    alt:'speaker-3',
                    name:'Angelina holy',
                    role:"Maxii's Managar"
                }
                
            ]
        }
    }
}
</script>
<style lang="scss">
#speakers{
    background-color: #F3F3F3;
    height: 500px;
    .controls{
        padding-top: 50px;
        .btn_angle{
        background-color: red;   
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
    background-color: red;
}
.square{
    height: 70px;
    width: 70px;
    border: 3px solid white;
    display: flex;
    align-items: center;
    justify-content: center;
}
</style>