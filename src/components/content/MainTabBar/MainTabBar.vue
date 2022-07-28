<template>
  <tab-bar>
    <tab-bar-item path="/home">
      <img slot="item-icon" src="~assets/img/tabbar/homeNoClick.png" />
      <img slot="item-icon-active" src="~assets/img/tabbar/home.png" />
      <div slot="item-text">首页</div>
    </tab-bar-item>
    <tab-bar-item path="/category">
      <img slot="item-icon" src="~assets/img/tabbar/classNoClick.png" />
      <img slot="item-icon-active" src="~assets/img/tabbar/class.png" />
      <div slot="item-text">分类</div>
    </tab-bar-item>
    <tab-bar-item path="/cart">
      <img slot="item-icon" src="~assets/img/tabbar/shopCarNoClick.png" />
      <img slot="item-icon-active" src="~assets/img/tabbar/shopCar.png" />
      <div slot="item-text">购物车</div>
    </tab-bar-item>
    <tab-bar-item path="/profile">
      <img slot="item-icon" src="~assets/img/tabbar/mineNoClick.png" />
      <img slot="item-icon-active" src="~assets/img/tabbar/mine.png" />
      <div slot="item-text">我的</div>
    </tab-bar-item>
  </tab-bar>
</template>

<script>
import TabBar from 'components/common/tabbar/TabBar.vue'
import TabBarItem from 'components/common/tabbar/TabBarItem.vue'

export default {
  name: 'MainTabBar',
  components: {
    TabBar,
    TabBarItem,
  },
}
</script>

<style></style>
