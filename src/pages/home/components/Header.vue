<template>
  <div class="header">
    <div class="header-left">
      <span class="iconfont">&#xe624;</span>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>
      输入城市/景点/游玩主题
    </div>
    <div class="header-right">
      城市
      <span class="iconfont">&#xe6aa;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style lang="stylus" scoped>
  .header
    display: flex
    line-height: .86rem
    background-color: #00bcd4
    color: #fff
    .header-left
      width: .664rem
      float: left
    .header-input
      flex: 1
      margin-top: .12rem
      margin-left: .2rem
      height: .64rem
      line-height: .64rem
      color: #ccc
      background-color: #fff
      border-radius: .1rem
    .header-right
      width: 1.24rem
      float: right
      text-align: center
</style>
