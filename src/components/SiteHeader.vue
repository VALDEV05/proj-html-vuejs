<template>
  <div id="siteHeader">
      <div class="container">
        <nav class="nav_header d-flex align-items-center justify-content-between">
            <div class="logo_header ms-1s">
                <Logo />
            </div>
            <div id="menu_header">
                <ul class="list-unstyled d-flex mt-3">
                    <li class="px-3" v-for="item in items" :key="item.element">
                        <a href="#" class="text-uppercase link_header text-decoration-none">{{item.element.toUpperCase()}}</a>
                    </li>
                    <!-- end cycle header -->
                    <li id="separate" class="px-3">|</li>
                    <li class="px-3"><a class="text-uppercase link_header text-decoration-none" href="#"><img src="@/assets/img/search-solid.svg" alt=""></a></li>
                </ul>
            </div>

        </nav>
      </div>
  </div>
    <!-- /siteHeader -->
</template>

<script>
import Logo from '../components/Logo.vue'
export default {
    props:{
        items: Array,
    },
    components:{
        Logo,
    }
}
</script>

<style  lang="scss">
.nav_header{
    height: 100px;
    width: 100%;
    a img{
        height: 15px;
        width: 15px;
    }
}    


</style>