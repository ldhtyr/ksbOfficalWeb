<!--
 * @FileDescription: 联系我们
 * @Author: ycl
 * @Date: ‎2021‎年‎9月‎9‎日 ‏‎
 * @LastEditors: ycl
 * @LastEditTime: 2021‎年‎9‎月‎9‎日
 -->
<template>
  <div class="box">
    <div class="headImg">
      <img
        src="../../assets/img/Connect-header.png"
        alt="auoutUs"
        class="img1"
      />
    </div>
    <div class="line">
      <p class="title">联系我们</p>
      <div class="lineBox">
        <div class="lineLong"></div>
        <div class="lineShort"></div>
      </div>
    </div>
    <div class="main">
      <div class="connectLeft">
        <img src="../../assets/img/Connect-map.png" alt="" />
      </div>
      <div class="connectRight">
        <div>
          <p class="conectTitle">北京凯思博科技有限公司</p>
          <div class="conectLine"></div>
        </div>
        <div class="list" style="margin-top:40px">
          <div style="margin-right: 150px;">
            <img
              src="../../assets/img/Connect-phone.png"
              alt=""
              class="listImg"
            />
            <span class="listTitle">公司电话</span>
            <p class="listContent">86-10-87227898</p>
          </div>
          <div>
            <img
              src="../../assets/img/Connect-phone.png"
              alt=""
              class="listImg"
            />
            <span class="listTitle">公司电话</span>
            <p class="listContent">86-10-87227898</p>
          </div>
        </div>
        <hr />
        <div style="margin-top: 36px;">
          <img
            src="../../assets/img/Connect-internet.png"
            alt=""
            class="listImg"
          />
          <span class="listTitle">公司网址</span>
          <p class="listContent">{{ `http://www.ksbps.cn/index.html` }}</p>
        </div>
        <hr />
        <div style="margin-top: 36px;">
          <img
            src="../../assets/img/Connect-email.png"
            alt=""
            class="listImg"
          />
          <span class="listTitle">公司邮箱</span>
          <p class="listContent">Service@kseiburg.c</p>
        </div>
        <hr />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "News",
};
</script>

<style scoped>
ul,
li {
  padding: 0;
  margin: 0;
  list-style-type: none;
}
.box {
  padding: 0;
  margin: 0;
  display: flex;
  flex-direction: column;
}
.img1 {
  width: 100%;
  height: 600px;
}
.lineLong {
  width: 100%;
  height: 2px;
  background-color: #d4d4d4;
}
.lineShort {
  width: 118px;
  height: 2px;
  position: absolute;
  top: 31px;
  left: 47%;
  background-color: #ff3a2f;
}
.title {
  font-size: 24px;
  font-weight: 400;
  color: #ff3a2f;
  text-align: center;
}
.headImg {
  padding: 0;
  margin: 0;
  width: 100%;
  height: 600px;
  /* border: 1px solid skyblue; */
}
.line {
  position: relative;
  margin-top: 120px;
}
.main {
  padding: 80px 375px;
  display: flex;
  /* justify-content: center;
  align-items: center; */
}
.connectRight {
  width: 560px;
  height: 500px;
  /* background-color: #f90; */
  padding: 32px 0px 32px 60px;
  box-sizing: border-box;
}
.conectLine {
  width: 60px;
  height: 1px;
  background: #dbdbdb;
  margin-top: 24px;
}
.conectTitle {
  font-size: 24px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #333333;
  line-height: 24px;
}
.list {
  width: 550px;
  /* height: 122px; */
  display: flex;
  justify-content: start;
  align-items: center;
}

.listTitle {
  font-size: 20px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #333333;
  line-height: 24px;
}
.listContent {
  font-size: 20px;
  font-family: Arial;
  font-weight: 400;
  color: #333333;
  line-height: 24px;
  margin-top: 10px;
  margin-bottom: 32px;
}
.listImg {
  margin-right: 10px;
}
</style>
