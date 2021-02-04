<template>
  <div>
    <TabBar>
       <TabBaritem path="/home" activecolor="deepPink">
         <img slot="item-icon" src="~assets/img/tabbar/home.svg" alt="">
         <img slot="item-active-icon" src="~assets/img/tabbar/home-active.svg" alt="">
         <div slot="item-text" >首页</div>
       </TabBaritem>
      <TabBaritem path="/category" activecolor="deepPink">
         <img slot="item-icon" src="~assets/img/tabbar/catroy.svg" alt="">
         <img slot="item-active-icon" src="~assets/img/tabbar/catroy-active.svg" alt="">
         <div slot="item-text">分类</div>
       </TabBaritem>
       <TabBaritem path="/cart" activecolor="deepPink">
         <img slot="item-icon" src="~assets/img/tabbar/shopping.svg" alt="">
         <img slot="item-active-icon" src="~assets/img/tabbar/shop-active.svg" alt="">
         <div slot="item-text">购物车</div>
       </TabBaritem>
       <TabBaritem path="/profile" activecolor="deepPink">
         <img slot="item-icon" src="~assets/img/tabbar/profile.svg" alt="">
         <img slot="item-active-icon" src="~assets/img/tabbar/profile-active.svg" alt="">
         <div slot="item-text">我的</div>
       </TabBaritem>
    </TabBar>
  </div>
</template>


<script>
 import TabBar from "./tabbar/TabBar"
 import TabBaritem from "./tabbar/TabBaritem"

export default {
  name: 'MainTabBar',
   components:{
     TabBar,
     TabBaritem
   }
}
</script>


<style scoped>

</style>
