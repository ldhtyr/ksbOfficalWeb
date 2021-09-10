<!--
 * @FileDescription: 新闻中心
 * @Author: ycl
 * @Date: ‎2021‎年‎9月‎9‎日 ‏‎
 * @LastEditors: ycl
 * @LastEditTime: 2021‎年‎9‎月‎9‎日
 -->
<template>
  <div class="box">
    <div class="headImg">
      <img src="../../assets/img/news-header.png" alt="auoutUs" class="img1" />
    </div>
    <div class="line">
      <p class="title">新闻中心</p>
      <div class="lineBox">
        <div class="lineLong"></div>
        <div class="lineShort"></div>
      </div>
    </div>
    <div class="newsMain">
      <div class="newsList">
        <div class="newsItem" v-for="(item, index) in list" :key="index">
          <div>
            <img :src="item.url" class="newsImg"/>
          </div>
          <div class="newsTitle">{{ item.title }}</div>
          <span class="newsTime">{{ item.time }}</span>
          <p class="newsContent">{{ item.content }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import news1 from "../../assets/img/news-1.png";
import news2 from '../../assets/img/news-2.png'
import news3 from '../../assets/img/news-3.png'
import news4 from '../../assets/img/news-4.png'
import news5 from '../../assets/img/news-5.png'
import news6 from '../../assets/img/news-6.png'
import news7 from '../../assets/img/news-7.png'
import news8 from '../../assets/img/news-8.png'
export default {
  name: "News",
  data() {
    return {
      list: [
        {
          title: "公安部多功能厅演3系统",
          time: "项目时间：2016-08-19",
          content: "承接并完成公安部边防管理局多功能厅演唱音响及灯光系统项目",
          url: news1,
        },
        {
          title:'白石山大剧院项目项',
          time:'项目时间：2016-08-19',
          content:'大型奇幻歌舞剧《白石山传奇》在保定涞源白石山大剧院震撼上演',
          url:news2
        },
        {
          title:'北京丰台王佐佃起文化活动中心设备采购',
          time:'项目时间：2016-08-19',
          content:'承接北京丰台王佐佃起文化活动中心设备采购项目',
          url:news3
        },
        {
          title:'北京丰台王佐佃起文化活动中心设备采购',
          time:'项目时间：2016-08-19',
          content:'承接北京丰台王佐佃起文化活动中心设备采购项目',
          url:news4
        },
        {
          title:'公安部多功能厅演系统',
          time:'项目时间：2016-08-19',
          content:'承接并完成公安部边防管理局多功能厅演唱音响及灯光系统项目',
          url:news5
        },
        {
          title:'白石山大剧院项目项',
          time:'项目时间：2016-08-19',
          content:'大型奇幻歌舞剧《白石山传奇》在保定涞源白石山大剧院震撼上演',
          url:news6
        },
        {
          title:'北京丰台王佐佃起文化活动中心设备采购',
          time:'项目时间：2016-08-19',
          content:'承接北京丰台王佐佃起文化活动中心设备采购项目',
          url:news7
        },
        {
          title:'北京丰台王佐佃起文化活动中心设备采购',
          time:'项目时间：2016-08-19',
          content:'承接北京丰台王佐佃起文化活动中心设备采购项目',
          url:news8
        },
      ],
    };
  },
};
</script>

<style scoped>

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
.newsMain{
  padding:50px 100px
}
.newsList{
  width: 1408px;
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}
.newsImg{
  width: 100%;
}
.newsItem {
  padding: 25px;
  width: 270px;
  height: 396px;
  border: 1px solid #eeeeee;
  margin-right: 30px;
  margin-bottom: 30px;
}
.newsTitle{

font-size: 18px;
font-family: Microsoft YaHei;
font-weight: 400;
color: #333333;
line-height: 27px;
}
.newsTime{

font-size: 14px;
font-family: Microsoft YaHei;
font-weight: 400;
color: #999999;
line-height: 27px;
}
.newsContent{
width: 219px;
height: 33px;
font-size: 14px;
font-family: Microsoft YaHei;
font-weight: 400;
color: #666666;
line-height: 21px;
}
.newsContent:hover{
  text-decoration: underline;
}
</style>
