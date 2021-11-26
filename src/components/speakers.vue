<template>
  <div class="container">
            <div class="controls d-flex justify-content-between">
                <div class="title_control">
                    <h1 class="text-uppercase fw-bold">Speakers</h1>
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
                    <div class="col-3">
                        <div class="card border-0" style="width: 18rem;">
                            <img src="@/assets/img/speaker-6.jpg" class="card-img-top" alt="speaker-6">
                            <div class="text_card text-center pt-3">
                                <p class="m-0 title-card text-uppercase">Patrick spencer</p>
                                <p class="m-0 subtitle-card">S&amp;P Analyzer</p>
                            </div>
                        </div>
                        <!-- /card -->
                    </div>
                    <!-- /col-card -->
                    <div class="col-3">
                        <div class="card border-0" style="width: 18rem;">
                            <img src="@/assets/img/speaker-5.jpg" class="card-img-top" alt="speaker-6">
                            <div class="text_card text-center pt-3">
                                <p class="m-0 title-card text-uppercase">Janet jones</p>
                                <p class="m-0 subtitle-card">Maxii's Managar</p>
                            </div>
                        </div>
                        <!-- /card -->
                    </div>
                    <!-- /col-card -->
                    <div class="col-3">
                        <div class="card border-0" style="width: 18rem;">
                            <img src="@/assets/img/speaker-4.jpg" class="card-img-top" alt="speaker-6">
                            <div class="text_card text-center pt-3">
                                <p class="m-0 title-card text-uppercase">Michael dover</p>
                                <p class="m-0 subtitle-card">Starbuck's CEO</p>
                            </div>
                        </div>
                        <!-- /card -->
                    </div>
                    <!-- /col-card -->
                    <div class="col-3">
                        <div class="card border-0" style="width: 18rem;">
                            <img src="@/assets/img/speaker-3.jpg" class="card-img-top" alt="speaker-6">
                            <div class="text_card text-center pt-3">
                                <p class="m-0 title-card text-uppercase">Angelina holy</p>
                                <p class="m-0 subtitle-card">Maxii's Managar</p>
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

}
</script>

<style lang="scss">
@import '@/assets/style/variables.scss';

#speakers{
    background-color: #F3F3F3;
    height: 500px;
    .controls{
        padding-top: 50px;
        .btn_angle{
        background-color: $scarlet-red-color;   
        height: 30px;
        width: 30px;
        padding: 20px;
        margin: 5px;
        display: flex;
        align-items: center;
        justify-content: center;
        color: $white-color;
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
                font-family: 'Bitter', serif;
                color: $icon-gray;
            }
        }
}


</style>