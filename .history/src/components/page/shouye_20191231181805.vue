<template>
  <div>
      <MainNav></MainNav>
      <!-- banner -->
      <swiper :options="swiperOption" ref="mySwiper">
        <!-- slides -->
        <swiper-slide>
          <div class="banner-item">
            <img src="../../assets/images/banner/banner2.png" alt="">
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="banner-item">
            <img src="../../assets/images/banner/banner2_2.png" alt="">
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="banner-item">
            <img src="../../assets/images/banner/banner2_3.png" alt="">
          </div>
        </swiper-slide>
        <!-- Optional controls -->
        <!-- <div class="swiper-pagination" slot="pagination"></div> -->
        <!-- <div class="swiper-scrollbar index-banner-circle" slot="scrollbar"></div> -->
      </swiper>
      <!-- 滚动公告 -->
      <Notice></Notice>
      <!-- 推荐分类栏 -->
      <div>
        <el-row>
          <el-tabs type="border-card">
            <el-tab-pane label="推荐">推荐</el-tab-pane>
            <el-tab-pane label="数码">数码</el-tab-pane>
            <el-tab-pane label="奖金">奖金</el-tab-pane>
            <el-tab-pane label="生活精品">生活精品</el-tab-pane>
            <el-tab-pane label="奢华品">奢华品</el-tab-pane>
            <el-tab-pane label="奢华品">奢华品</el-tab-pane>
          </el-tabs>
        </el-row>
      </div>
  </div>
</template>
<script>
import MainNav from '@/components/page/MainNav'
import Notice from '@/components/page/Notice'
import {swiper, swiperSlide} from 'vue-awesome-swiper'

export default {
  name: 'App',
  components: {
    MainNav,
    swiper,
    swiperSlide,
    Notice
  },
  data () {
    return {
      swiperOption: {
        scrollbar: {
          el: '.swiper-scrollbar'
        },
        slidesPerView: 1,
        autoplay: {
          delay: 3000000,
          disableOnInteraction: false
        },
        loop: true
      }
    }
  }
}
</script>
<style>
/* .swiper-container{
  height: 100%;
  margin-bottom: -4px;
} */
/* .el-tabs__item{
  padding: 0 5.26% !important;
} */
.el-tabs__nav{
  width: 100%
}
.el-tabs--border-card{
  border: 0;
}
.el-tabs--border-card>.el-tabs__header .el-tabs__item{
  border: 0
}
.el-tabs--border-card>.el-tabs__header{
  padding: 10px 15px 0;
  background: #151515
}
.el-tabs--border-card>.el-tabs__header .el-tabs__item:not(.is-disabled):hover{
  color: #ffffff;
}
.el-tabs--border-card>.el-tabs__header .el-tabs__item.is-active{
  height: 39px;
  color: #ffffff;
  background: #292C35;
}
.el-tabs--border-card>.el-tabs__header .el-tabs__item{
  color: #666666;
}
</style>
