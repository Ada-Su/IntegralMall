<template>
  <div class="top-nav">
    <div class="top-nav-left">
      <img src="../../assets/images/topnav/cd.png" alt="菜单">
    </div>
    <div class="top-nav-t">
      <p>VIP权益</p>
    </div>
    <div class="top-nav-right">
      <img src="../../assets/images/topnav/ss.png" alt="搜索">
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      tabBarImgArr: [
        {normal: require('../../assets/images/topnav/logo.png')},
        {normal: require('../../assets/images/topnav/ss.png')},
        {normal: require('../../assets/images/topnav/cd.png')}
      ]
    }
  }
}
</script>
<style>

</style>
