<template>
  <div class="hello">
    <div class="header">
      <div class="left">
        <img src="static\img\Back.png" class="back">
      </div>
      <div class="center">页面名称</div>
      <div class="right">
        <img src="static\img\全局操作.png" class="caozuo">
      </div>
    </div>

    <div class="img">
      <x-img
        src="static\img\1.png"
        @on-success="success"
        @on-error="error"
        class="ximg-demo"
        error-class="ximg-error"
        :offset="-100"
        container="#vux_view_box_body"
      ></x-img>
      <div class="wenzi">
        <p class="wanju">玩具反斗城</p>
        <p class="zhekou">员工折扣卡</p>
        <p class="cardid">9523245</p>
      </div>
    </div>
<div class="erweima">
       <img src="static\img\2.png">
      
</div>
<p class="haoma">
    958976654
</p>
  <hr>
 
  <div>
      <div class="wanjufan">
          玩具反斗城商城
      </div>
      <div class="jinqu">
          进去逛逛>
      </div>
  </div>
  </div>
</template>

<script>
import {
  XHeader,
  XImg,
  Actionsheet,
  TransferDom,
  ButtonTab,
  ButtonTabItem
} from "vux";

export default {
  name: "HelloWorld",
  components: {
    XHeader,
    Actionsheet,
    ButtonTab,
    ButtonTabItem,
    XImg
  },
  methods: {
    success(src, ele) {
      console.log("success load", src);
    },
    error(src, ele, msg) {
      console.log("error load", msg, src);
    }
  },
  data() {
    return {
      msg: "Welcome to Your Vue.js App"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.jinqu{
    margin-top: 42px;
    margin-left: 263px;
height:33px;
font-size:24px;
font-family:PingFangSC-Medium;
font-weight:500;
color:rgba(142,142,147,1);
line-height:33px;
float: left;
}
.wanjufan{
 margin-left: 62px;
height:50px;
font-size:36px;
font-family:PingFangSC-Medium;
font-weight:500;
color:#000000;
line-height:50px;
float: left;
margin-top: 34px;
}
hr{
    width: 624px;
    margin: 0 auto;
    margin-top: 80px;
}
.haoma{
 text-align: center;
height:70px;
font-size:48px;
font-family:PingFangSC-Regular;
font-weight:400;
color:rgba(0,0,0,1);
line-height:67px;
letter-spacing:5px;
margin-top: 10px;
}
.right{
  float: left;
 padding-top: 8px;
background:rgba(255,255,255,1);
margin-left: 113px;
display: flex;
align-items: center;
justify-content: center;
}
.right img{
 width:174px;

}
.center {
  padding-top: 18px;
  margin-left: 242px;
  height: 52px;
  font-size: 37px;
  font-family: PingFangSC-Medium;
  font-weight: 500;
  color: rgba(0, 0, 0, 1);
  line-height: 52px;
  float: left;
}
.left {
  width: 36px;
  padding-top: 26px;
  margin-left: 23px;
  float: left;
}
.back {
  width: 23px;
  height: 36px;
}
.header {
  height: 88px;
}
.btn {
  margin-top: 328px;
  width: 625px;
  height: 94px;
  background: rgba(89, 86, 214, 1);
  border-radius: 10px;
  border: 2px solid rgba(5, 5, 5, 0.08);
  margin-left: 63px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 151px;
}
.cardid {
  margin-top: 212px;

  height: 28px;
  font-size: 20px;
  font-family: PingFangSC-Regular;
  font-weight: 400;
  color: rgba(208, 209, 234, 1);
  line-height: 28px;
}
.wenzi {
  position: absolute;
  top: 30px;
  left: 93px;
}
.zhekou {
  margin-top: 10px;

  height: 28px;
  font-size: 20px;

  font-weight: 400;
  color: rgba(208, 209, 234, 1);
  line-height: 28px;
}
.erweima{
    width: 100%;
    margin-top: 80px;
    display: flex;
    align-items: center;
    justify-content: center;
}
.erweima img{
    width: 400px;
}
.img {
  width: 100%;
  display: flex;
  align-items: center;
  position: relative;
  margin-top: 60px;
}
.wanju {
  height: 42px;
  font-size: 30px;
  font-weight: 600;
  color: rgba(208, 209, 234, 1);
  line-height: 42px;
  letter-spacing: 1px;
}
.vux-x-img {
  width: 624px;
  margin: 0 auto;
}
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
