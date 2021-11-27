<template>
<div class="d-flex justify-content-center" style="width:100vw; height:300px;">
    <GmapMap
            :center="{lat:51.507437, lng:-0.127265}"
            :zoom="14"
            map-type-id="terrain"
            style="width: 100vw; height: 300px"
>
  <GmapMarker
    :key="index"
    v-for="(m, index) in markers"
    :position="m.position"
    :clickable="true"
    :draggable="true"
    @click="center=m.position"
  />
</GmapMap>
</div>

</template>

<script>

export default {
    data(){
        return{
            markers:[
                {
                    position:{
                        lat:51.507437, lng:-0.127265
                    },
                }
            ]
        }
    }

}
</script>

<style>

</style>