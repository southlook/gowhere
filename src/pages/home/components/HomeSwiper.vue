<template>
    <div class="wrapper">
        <swiper :options="swiperOption">
            <swiper-slide v-for="item of swiperList" :key="item.id">
                <img class="swiper-img" :src="item.imgUrl" />
            </swiper-slide>
            <div class="swiper-pagination" slot="pagination"></div>
        </swiper>
    </div>
</template>

<script>
    export default {
        name:'HomeSwiper',
        data(){
            return {
                swiperOption:{
                    pagination:'.swiper-pagination',
                    loop:true,
                    autoplay:3000
                },
                swiperList:[{
                    id:'0001',
                    imgUrl:'https://tr-osdcp.qunarzz.com/tr-osd-vs-dapp-ugc/img/9bc953039cf4a3e6af7adbdbb3aa6dc6.jpg'
                },{
                    id:'0002',
                    imgUrl:'https://tr-osdcp.qunarzz.com/tr-osd-vs-dapp-ugc/img/be049a68a045fa43ecc1044e5bbbd343.jpg'
                }]
            }
        }
    }
</script>

<style lang="stylus" scoped>
   .wrapper >>> .swiper-pagination-bullet-active
    background:#fff!important
   .wrapper
    overflow:hidden
    width:100%
    height:0
    padding-bottom:31.25%
    background:#eee
   
   .swiper-img
     width:100%
</style>