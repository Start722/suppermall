<template>
<div class="detail-bottom">
  <div class="bar-item bar-left">
    <div>
      <img class="icon select" src="~assets/img/detail/comment.png">
      <span class="text">客服</span>
    </div>
    <div>
      <img class="icon select" src="~assets/img/detail/shop.png">
      <span class="text">店铺</span>
    </div>
    <div>
      <img class="icon select" src="~assets/img/detail/serve.png">
      <span class="text">收藏</span>
    </div>
  </div>
  <div class="bar-item bar-right">
    <div class="cart" @click="addToCart">加入购物车</div>
    <div class="buy">购买</div>
  </div>
</div>
</template>

<script>
export default {
  name: "DetailBottomBar",
  methods: {
    addToCart(){
     this.$emit('addcart')
    }
  }
}
</script>

<style scoped>
.detail-bottom{
  height: 55px;
  position: fixed;
  background-color: #fff;
  left: 0;
  right: 0;
  bottom: 0;
  display: flex;
  text-align: center;
}
.bar-item {
  flex: 1;
  display: flex;
}
.bar-item>div {
  flex: 1;
}
.bar-left .text {
  font-size: 13px;
}
.bar-left .icon {
  display: block;
  width: 22px;
  height: 22px;
  margin: 10px auto 3px;
}
.bar-left .service {
  background-position:0 -54px;
}
.bar-left .shop {
  background-position:0 -98px;
}
.bar-right {
  font-size: 15px;
  color: #fff;
  line-height: 58px;
}
.bar-right .cart {
  background-color: rgb(255, 238, 0);
  color: #333;
}
.bar-right .buy {
  background-color: coral;
}
</style>