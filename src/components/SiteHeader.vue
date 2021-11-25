<template>
  <div id="siteHeader">
      <div class="container">
        <nav class="nav_header d-flex align-items-center justify-content-between">
            <div class="logo_header ms-1s">
                <Logo />
            </div>
            <div id="menu_header">
                <ul class="list-unstyled d-flex mt-3">
                    <li class="px-3"><a class="text-uppercase link_header text-decoration-none" href="#">home</a></li>
                    <li class="px-3"><a class="text-uppercase link_header text-decoration-none" href="#">pages</a></li>
                    <li class="px-3"><a class="text-uppercase link_header text-decoration-none" href="#">program</a></li>
                    <li class="px-3"><a class="text-uppercase link_header text-decoration-none" href="#">tickets</a></li>
                    <li class="px-3"><a class="text-uppercase link_header text-decoration-none" href="#">speakers</a></li>
                    <li class="px-3"><a class="text-uppercase link_header text-decoration-none" href="#">papers</a></li>
                    <li class="px-3"><a class="text-uppercase link_header text-decoration-none" href="#">blog</a></li>
                    <li class="px-3"><a class="text-uppercase link_header text-decoration-none" href="#">shortcodes</a></li>
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
        title:String,
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