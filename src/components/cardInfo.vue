<template>
  <div class="section_card container">
        <div class="row mt-5">
            <div class="col card_main d-flex" v-for="item in items" :key="item.index">
                <img :src="require('@/assets/img/' + item.imageUrl)" :alt="item.altImage">
                <div id="text_card" class="mx-4">
                    <p class="title_card text-uppercase">{{item.title}}</p>
                    <p class="text-muted">{{item.text}}</p>
                    <p><a href="#" class="learn_more_font">{{item.link}}</a></p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props:{
            items:Array,
        }
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