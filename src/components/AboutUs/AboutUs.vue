<!--
 * @FileDescription: 关于我们
 * @Author: ycl
 * @Date: ‎2021‎年‎9月‎9‎日 ‏‎
 * @LastEditors: ycl
 * @LastEditTime: 2021‎年‎9‎月‎9‎日
 -->
<template>
  <div>
    <div class="box">
      <!-- 头部图片 -->
      <div class="headImg">
        <img
          src="../../assets/img/AboutUs-header.png"
          alt="auoutUs"
          class="img1"
        />
      </div>
      <div class="line">
        <p class="title">公司介绍</p>
        <div class="lineBox">
          <div class="lineLong"></div>
          <div class="lineShort"></div>
        </div>
      </div>
      <!-- 公司介绍 -->
      <div class="introduce">
        <div class="introduceLeft">
          <img src="../../assets/img/AboutUs-introduce-left.png" />
        </div>
        <div class="introduceRight">
          <div class="introduceTitle">公司介绍</div>
          <div class="introduceMain">
            北京凯思博科技有限公司是国家高新技术企业，中关村高新技术企业。
            总部位于北京亦庄经济开发区，在全国各地设有分支机构。依托团队在电力
            电子，锂电池、工业物联网领域的长期积累，致力于为客户提供创新型的数字
            能源解决方案，提升客户整体能源资产的运营效率。
            Kseiburg”为公司的注册商标。秉持“提升能源资产运营效率，助力企业数
            字化转型”的使命，致力于成为能源物联网领域的标杆企业。
            公司积累了数十项专利及软件著作权，通过了ISO9001质量管理体系认证，I
            SO14001环境管理体系认证，ISO45001职业健康安全管理体系等认证。公司服务行
            业包括：石油石化，半导体，电信，金融，交通等领域。
          </div>
        </div>
      </div>
      <div class="line" style=" margin-top: 100px;">
        <p class="title">凯思博团队</p>
        <div class="lineBox">
          <div class="lineLong"></div>
          <div class="lineShort"></div>
        </div>
      </div>
      <!-- 团队 -->
      <div class="team">
        <img src="../../assets/img/AboutUs-team.png" class="img1" />
        <div class="backGround">
          <div
            v-for="(item, index) in list"
            :key="index"
            class="backGroundItem"
          >
            <div class="chinese">{{ item.Chinese }}</div>
            <div class="english">{{ item.English }}</div>
          </div>
        </div>
      </div>
      <div class="line">
        <p class="title">工会活动</p>
        <div class="lineBox">
          <div class="lineLong"></div>
          <div class="lineShort"></div>
        </div>
      </div>
      <!-- 活动 -->
      <div class="activity">
        <div class="act">
          <div v-for="(item, index) in activity" :key="index" class="actItem">
            <div class="actImg">
              <img :src="item.url" />
            </div>
            <div class="actTitle">{{ item.name }}</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import actLeft from "../../assets/img/AboutUs-act-left.png";
import actMiddle from "../../assets/img/AboutUs-act-middle.png";
import actRight from "../../assets/img/AboutUs-act-right.png";
export default {
  name: "AboutUs",
  data() {
    return {
      list: [
        {
          Chinese: "创新",
          English: "INNOVATION",
        },
        {
          Chinese: "诚信",
          English: "INTEGRITY",
        },
        {
          Chinese: "开拓",
          English: "DEVELOPING",
        },
        {
          Chinese: "真情",
          English: "TRUTH",
        },
      ], //黑色蒙层数据
      activity: [
        {
          name: "晚会活动",
          url: actLeft,
        },
        {
          name: "灯会活动",
          url: actMiddle,
        },
        {
          name: "讲座活动",
          url: actRight,
        },
      ], //工会活动数据
    };
  },
  methods: {},
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

.introduce {
  width: 100%;
  height: 438px;
  /* background-color: #f90; */
  display: flex;
  justify-content: space-evenly;
  align-items: flex-end;
}
.introduceTitle {
  margin-bottom: 43px;
  height: 24px;
  font-size: 24px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #333333;
  line-height: 24px;
}
.introduceMain {
  width: 669px;
  height: 234px;
  font-size: 18px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #666666;
  line-height: 27px;
}

.team {
  margin-top: 79px;
  width: 100%;
  height: 600px;
  position: relative;
}
.backGround {
  width: 1170px;
  height: 103px;
  position: absolute;
  bottom: 0;
  right: 21%;
  display: flex;
  justify-content: space-around;
  align-items: center;
  background-color: #000;
  opacity: 0.85;
}
.backGroundItem {
  width: 100px;
}
.chinese {
  font-size: 24px;
  font-family: Microsoft YaHei;
  font-weight: bold;
  color: #fff;
  line-height: 24px;
  text-align: center;
}
.english {
  font-size: 14px;
  text-align: center;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #fff;
  line-height: 27px;
  text-align: center;
}

.activity {
  width: 100%;
  height: 612px;
  padding-top: 80px;
  /* background-color: green; */
}
.act {
  display: flex;
  justify-content: center;
  align-items: center;
}
.actItem {
  margin-right: 30px;
}
.actTitle {
  padding-top: 50px;
  font-size: 18px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #666666;
  line-height: 24px;
  text-align: center;
}
</style>
