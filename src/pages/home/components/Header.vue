<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">&#xe624;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>
      输入城市/景点/游玩主题
    </div>
    <router-link to="/city">
      <div class="header-right">
        {{ this.city }}
        <span class="iconfont">&#xe6aa;</span>
      </div>
    </router-link>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {
    city: String
  }
}
</script>

<style lang="stylus" scoped>
  @import "~style/varibles.styl"
  .header
    display flex
    line-height $headerHeight
    background-color $bgColor
    color #fff
    .header-left
      width .664rem
      float left
      .back-icon
        text-align center
        font-size .4rem
    .header-input
      flex 1
      margin-top .12rem
      margin-left .2rem
      padding-left .2rem
      height .64rem
      line-height .64rem
      color #ccc
      background-color #fff
      border-radius .1rem
    .header-right
      width 1.24rem
      float right
      text-align center
      color white
</style>
