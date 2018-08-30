<template>
  <div>
    <div class="title">热销推荐</div>
    <ul>
      <li class="item border-bottom" v-for="item of recommendList" :key="item.id">
        <img class="item-img"
             :src="item.imgUrl">
        <div class="item-info">
          <p class="item-title">{{item.title}}</p>
          <p class="item-desc">{{item.desc}}</p>
          <button class="item-button">查看详情</button>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      recommendList: [
        {
          id: '0001',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1505/be/be4802e10f3b3107.water.jpg_200x200_0e98aabe.jpg',
          title: '武隆天坑地缝国家地质公园',
          desc: '武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩'
        },
        {
          id: '0002',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1505/be/be4802e10f3b3107.water.jpg_200x200_0e98aabe.jpg',
          title: '武隆天坑地缝国家地质公园',
          desc: '武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩'
        },
        {
          id: '0003',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1505/be/be4802e10f3b3107.water.jpg_200x200_0e98aabe.jpg',
          title: '武隆天坑地缝国家地质公园',
          desc: '武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩'
        },
        {
          id: '0004',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1505/be/be4802e10f3b3107.water.jpg_200x200_0e98aabe.jpg',
          title: '武隆天坑地缝国家地质公园',
          desc: '武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩'
        },
        {
          id: '0005',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1505/be/be4802e10f3b3107.water.jpg_200x200_0e98aabe.jpg',
          title: '武隆天坑地缝国家地质公园',
          desc: '武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩'
        },
        {
          id: '0006',
          imgUrl: 'http://img1.qunarzz.com/sight/p0/1505/be/be4802e10f3b3107.water.jpg_200x200_0e98aabe.jpg',
          title: '武隆天坑地缝国家地质公园',
          desc: '武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩武隆天坑地缝国家地质公园很好玩'
        }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
  @import "~styles/mixins.styl"

  .title
    margin-top .2rem
    line-height .8rem
    background #eee
    text-indent .2rem

  .item
    overflow hidden
    display flex
    height 1.9rem
    .item-img
      width 1.7rem
      height 1.7rem
      padding .1rem
    .item-info
      flex 1
      min-width 0
      padding .1rem
      .item-title
        line-height .4rem
        font-size .32rem
        ellipse()
      .item-desc
        line-height .4rem
        color #ccc
        ellipse()
      .item-button
        line-height .44rem
        margin-top .2rem
        background #ff9300
        padding 0 .2rem
        border-radius .06rem
        color #fff

</style>
