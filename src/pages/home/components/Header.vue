<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont icon-fanhui back-icon"></div>
    </div>
    <div class="header-input">
      <span class="iconfont icon-sousuo"></span>
      输入城市/景点/游玩/主题</div>
    <router-link to="/city">
    <div class="header-right">{{city}}
      <span class="iconfont icon-jiantou arrow-icon"></span>
    </div>
    </router-link>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader',
  props: {
    city: String
  }
}
</script>

<style lang="stylus" scoped>
  @import '~styles/varibles.styl'
  .header
    display: flex
    $headerHeight
    background: $bgColor
    color: #ffffff
    .header-left
      width: .64rem
      float: left
      .back-icon
        text-align: center
        font-size: .4rem
    .header-input
      flex: 1
      height: .64rem
      line-height:.64rem
      margin-top: .12rem
      margin-left: .2rem
      padding-left: .2rem
      background #ffffff
      border-radius: .1rem
      color: #ccc
    .header-right
      width: 1.24rem
      float: right
      text-align: center
      color white
      .arrow-icon
        margin-left: -.04rem
        font-size: .24rem

</style>
