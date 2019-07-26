<template>
  <div class="wrapper">
         <swiper :options="swiperOption" >
    <swiper-slide v-for="item of swiperList" :key="item.id">
        <img class="swiper-img" :src="item.imgurl" alt="">
         
    </swiper-slide>
    
   
    <div class="swiper-pagination"  slot="pagination"></div>
  </swiper>
  </div>
</template>
<script>
export default {
    name:'HomeSwiper', 
    data(){
        return {
            swiperOption:{
                //轮播图点样式
                pagination: '.swiper-pagination' 
            },
            swiperList:[{
                id:'001',
                imgurl:'http://img0.bdstatic.com/static/searchresult/img/logo-2X_32a8193.png'
            },
            {
                  id:'002',
                imgurl:'http://img0.bdstatic.com/static/searchresult/img/logo-2X_32a8193.png'
            }
            ]
        }
    }
}
</script>
<style lang="stylus">

.swiper-pagination-bullet{
    background :#fff
}
.wrapper
    overflow :hidden
    width : 100%
    height : 0
    padding-bottom : 31.25%
    .swiper-img
        width : 100%
        
            
         
</style>
