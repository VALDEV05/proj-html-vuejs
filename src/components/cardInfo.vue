<template>
  <div class="section_card container">
        <div class="row mt-5">
            <div class="col card_main d-flex">
                <img src="@/assets/img/trophy-solid.svg" alt="trophy">
                <div id="text_card" class="mx-4">
                    <p class="title_card text-uppercase">Who we are</p>
                    <p class="text-muted">Donec id elit non mi porta gravida at eget me tus. Sed posuere consectutyr estat lobo rtis. Cum sociis natoque.</p>
                    <p><a href="#" class="learn_more_font">Learn More</a></p>
                </div>
            </div>
            <div class="col card_main d-flex">
                <img src="@/assets/img/bolt-solid.svg" alt="bolt">
                <div id="text_card" class="mx-4">
                    <p class="title_card text-uppercase">What we do</p>
                    <p class="text-muted">Donec id elit non mi porta gravida at eget me tus. Sed posuere consectutyr estat lobo rtis. Cum sociis natoque.</p>
                    <p><a href="#" class="learn_more_font">Learn More</a></p>
                </div>

            </div>
            <div class="col card_main d-flex">
                <img src="@/assets/img/question-solid.svg" alt="question">
                <div id="text_card" class="mx-4">
                    <p class="title_card text-uppercase">why us?</p>
                    <p class="text-muted">Donec id elit non mi porta gravida at eget me tus. Sed posuere consectutyr estat lobo rtis. Cum sociis natoque.</p>
                    <p><a href="#" class="text-decoration-none learn_more_font">Learn More</a></p>
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

.section_card {
    .card_main {
        width: 33.33%;
        img {
            height: 50px;
            width: 50px;
            color: $icon-gray;
        }
        #text_card {
            .title_card {
                font-size: 25px;
                font-weight: bold;
            }
            p a {
                text-decoration: none;
                color: $scarlet-red-color;
                font-family: 'Bitter', serif;
            }
        }
    }
}
</style>