<template>
  <div>
    <div class="recommend-title">热销推荐</div>
    <ul>
      <li
        class="item border-bottom"
        v-for="item of recommendList"
        :key="item.id">
        <img class="item-img" :src="item.imgUrl">
        <div class="item-info">
          <p class="item-title">{{ item.title }}</p>
          <p class="item-desc">{{ item.desc }}</p>
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
      recommendList: [{
        id: '0001',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_200x200_1bc99086.jpg',
        title: '故宫',
        desc: '北京首都'
      }, {
        id: '0002',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_200x200_1bc99086.jpg',
        title: '故宫',
        desc: '北京首都'
      }, {
        id: '0003',
        imgUrl: 'http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_200x200_1bc99086.jpg',
        title: '故宫',
        desc: '北京首都'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .recommend-title
    margin-top: .2rem
    line-height: .8rem
    background-color: #eee
    text-indent: .2rem
  .item
    display: flex
    height: 1.9rem
    overflow: hidden
    .item-img
      width: 1.7rem
      height: 1.7rem
      padding: .1rem
    .item-info
      flex: 1
      padding: .1rem
      .item-title
        line-height: .54rem
        font-size: .32rem
      .item-desc
        line-height: .4rem
        color: #ccc
      .item-button
        line-height: .44rem
        margin-top: .16rem
        background: #ff9300
        padding: .08rem
        border-radius: .06rem
        color: #fff
</style>
