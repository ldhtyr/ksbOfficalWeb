<template>
  <div class="">
    <div style="width:1903px; height=600px">
      <img
        style="width:1903px; height=600px"
        src="../assets/img/homePage_banner.png"
        alt=""
      />
    </div>
    <div style="width:1903px;height:650px">
      <div class="introductory">
        <div class="introductoryHead">
          <div class="size">企业简介</div>
          <div class="si">COMPANY PROFILE</div>
        </div>
        <div class="introductoryFoot">
          <div>
            <img
              style="width:570px;height:430px"
              src="../assets/img/homePage_back.png"
              alt=""
            />
          </div>
          <div class="companyIn">
            <div class="company">北京凯思博科技有限公司</div>
            <div>
              <div class="con">
                北京凯思博科技有限公司是国家高新技术企业，中关村高新技术企业。总部位于北京亦庄经济开发区，在全国各地设有分支机构。依托团队在电力电子，锂电池、工业物联网领域的长期积累，致力于为客户提供创新型的数字能源解决方案，提升客户整体能源资产的运营效率。
              </div>
              <div class="con">
                Kseiburg”为公司的注册商标。秉持“提升能源资产运营效率，助力企业数字化转型”的使命，致力于成为能源物联网领域的标杆企业。
              </div>
              <div class="con">
                公司积累了数十项专利及软件著作权，通过了ISO9001质量管理体系认证，ISO14001环境管理体系认证，ISO45001职业健康安全管理体系等认证。公司服务行业包括：石油石化，半导体，电信，金融，交通等领域。......
              </div>
            </div>
            <div class="more">
              <div style="color:#FF3A2F">>></div>
              <div class="mor">更多</div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div style="width:1903px;height:900px;background: #EDECEC;">
      <div class="new">
        <div class="introductoryHead">
          <div class="size">产品展示</div>
          <div
            style="
font-size: 18px;
color: #666666;"
          >
            Product display
          </div>
        </div>
      </div>
      <div class="option">
        <div
          @click="ModelChoce(index)"
          class="op"
          v-for="(item, index) in data"
          :key="index"
        >
          <div :style="ModelNum == index ? 'color:#FF3A2F' : ''">
            {{ item.name }}
          </div>
          <div :style="ModelNum == index ? 'color:#FF3A2F' : ''">
            {{ item.tit }}
          </div>
        </div>
      </div>

      <div class="swiper-container">
        <div class="swiper-wrapper">
          <div data-swiper-autoplay="1000" class="swiper-slide">
            <img
              style="width:350px;height:322px"
              src="../assets/img/SSU.png"
              alt=""
            />
          </div>
          <div data-swiper-autoplay="1000" class="swiper-slide">
            <img src="../assets/img/SMC.png" alt="" />
          </div>
          <div data-swiper-autoplay="1000" class="swiper-slide">
            <img src="../assets/img/BMD.png" alt="" />
          </div>
          <div data-swiper-autoplay="1000" class="swiper-slide">
            <img src="../assets/img/SMC.png" alt="" />
          </div>
          <div data-swiper-autoplay="1000" class="swiper-slide">
            <img src="../assets/img/BMD.png" alt="" />
          </div>
        </div>
        <div class="swiper-button-next"></div>
        <div class="swiper-button-prev"></div>
      </div>
    </div>
    <div style="width:1903px;height:750px;">
      <div class="new">
        <div class="introductoryHead">
          <div class="size">新闻中心</div>
          <div class="si">Information Centre</div>
        </div>
      </div>
      <div style="width:1200px;margin:auto">
        <div style="height:40px">
          <div style="font-size:24px;color: #FF3A2F;">新闻动态</div>
          <div
            style="margin-top:5px;width:1173px;height:1px;background: #D4D4D4;"
          >
            <div style="width:94px;height:1px;background: #C21F30;"></div>
            <div></div>
          </div>
        </div>
        <div class="newFo">
          <div style="width:455px;height:424px">
            <img
              style="width:455px;height:424px"
              src="../assets/img/homePage-new.png"
              alt=""
            />
          </div>
          <div class="newCon">
            <div
              @click="jump(0)"
              :class="jumps == 0 ? 'newConName' : 'newConNames'"
            >
              北京凯思博科技有限公司荣膺 “守诚信立商信示范单
            </div>
            <div style="display:flex;justify-content: space-between;">
              <div class="day">
                <div>2-1</div>
                <div>2020</div>
              </div>
              <div style="width:460px;color: #666666;font-size:14px">
                本报讯 （记者
                付永栋）在2020年2月1日召开的2019诚实守信道德模范颁奖盛典上，北京凯思博科技公司荣膺2019守诚信立商信示范单位称号，公司执行董事冯泽辉获评2019年度诚信。
              </div>
            </div>
            <div
              @click="jump(1)"
              :class="jumps == 1 ? 'newConName' : 'newConNames'"
            >
              北京凯思博科技有限公司开展“十九大”精神学习宣贯 “
            </div>
            <div style="display:flex;justify-content: space-between;">
              <div class="day">
                <div>11-17</div>
                <div>2019</div>
              </div>
              <div style="width:460px;color: #666666;font-size:14px">
                连日来，党的十九大报告在北京凯思博科技有限公司广大干部职工中引起强烈反响，公司上下掀起一场学习热潮。为了更深入地贯彻落实党的十九大报告精神，11月17日上午，公司党支部组织全体员工在5号楼四楼会议室对党的十九大报告进行了集中学习宣贯。
              </div>
            </div>
            <div
              @click="jump(2)"
              :class="jumps == 2 ? 'newConName' : 'newConNames'"
            >
              凯思博与中国石化进行工作交流
            </div>
            <div style="display:flex;justify-content: space-between;">
              <div class="day">
                <div>2-1</div>
                <div>2019</div>
              </div>
              <div style="width:460px;color: #666666;font-size:14px">
                本报讯
                6月19日，北京凯思博科技有限公司执行董事冯泽辉一行到中国石化有限公司进行工作交流。中国石化有限公司总经理韩某某与北京凯思博开机有限公司执行董事冯泽辉，经理郑林鹏达成深度合作。
              </div>
            </div>
            <div class="see">查看更多</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Swiper from "swiper";
export default {
  components: {},

  data() {
    return {
      ModelNum: 0,
      jumps: 0,
      data: [
        { name: "主控模块", tit: "SMCU" },
        { name: "感知模块", tit: "SSU" },
        { name: "显示屏", tit: "BM-D" },
        { name: "霍尔传感器", tit: "HS" },
        { name: "电路板", tit: "BM-Cutover" },
      ],
    };
  },
  computed: {},
  watch: {},
  methods: {
    jump(item) {
      this.jumps = item;
    },
    ModelChoce(index) {
      this.ModelNum = index;
    },
  },

  created() {},

  mounted() {
    var mySwiper = new Swiper(".swiper-container", {
      autoplay: {
        disableOnInteraction: false,
        pauseOnMouseEnter: true,
      },
      slidesPerView: 3,
      spaceBetween: 30,
      centeredSlides: true,
      // slidesPerGroup: 3,
      loop: true,
      // loopFillGroupWithBlank: true,
      // pagination: {
      //   el: ".swiper-pagination",
      //   clickable: true,
      // },
      navigation: {
        nextEl: ".swiper-button-next",
        prevEl: ".swiper-button-prev",
      },
    });
    mySwiper.el.onmouseover = function() {
      mySwiper.autoplay.stop();
    };
    mySwiper.el.onmouseout = function() {
      mySwiper.autoplay.start();
    };
  },
  props: [],
  beforeCreate() {},
  updated() {},
};
</script>
<style scoped>
/* @font-face {
  font-family: Microsoft YaHei;
  src: url("../assets/微软雅黑/msyhl.ttc");
} */
.swiper-container {
  --swiper-navigation-color: #333333; /* 单独设置按钮颜色 */
  --swiper-navigation-size: 30px; /* 设置按钮大小 */
  width: 1230px;
  height: 550px;
  margin-top: 100px;
  /* margin-left: auto;
  margin-right: auto; */
}
.swiper-slide {
  text-align: center;
  font-size: 18px;
  background: #fff;

  /* Center slide text vertically */
  display: -webkit-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  -webkit-justify-content: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  -webkit-align-items: center;
  align-items: center;
  transition: 300ms;
  transform: scale(0.8);
  height: 400px;
  /* margin-right: 0 !important; */
  border-radius: 20px;
  box-shadow: 3px 5px 5px #ccc;
}
.swiper-slide-active,
.swiper-slide-duplicate-active {
  transform: scale(1);
}
.swiper-button-prev,
.swiper-button-next {
  top: 37% !important;
}
.op {
  display: flex;
  height: 30px;
}
.op > div:nth-child(2) {
  /* width: 40px; */
  /* height: 10px; */
  font-size: 14px;
  font-family: Arial;
  font-weight: 400;
  color: #999999;
  line-height: 21px;
  margin-top: 5px;
  margin-left: 5px;
}
.op > div:nth-child(1) {
  /* width: 88px; */
  /* height: 22px; */
  font-size: 22px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #333333;
  line-height: 18px;
}
.option {
  width: 1200px;
  height: 40px;
  margin: auto;
  display: flex;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.see {
  width: 136px;
  height: 36px;
  background: #c21f30;
  border-radius: 4px;
  text-align: center;
  line-height: 36px;
  color: #fff;
  margin-left: 450px;
  cursor: pointer;
}
.day {
  width: 70px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  border-right: 1px solid #d4d4d4;
  color: #999999;
  font-size: 14px;
}
.newConName {
  /* width: 419px; */
  height: 18px;
  font-size: 18px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #c62e3e;
  margin-left: 90px;
  cursor: pointer;
}
.newConNames {
  /* width: 419px; */
  height: 18px;
  font-size: 18px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #333333;
  margin-left: 90px;
  cursor: pointer;
}
.newCon {
  width: 554px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
}
.newFo {
  display: flex;
  justify-content: space-between;
  margin-top: 30px;
}
.new {
  height: 200px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.mor {
  width: 36px;
  height: 18px;
  font-size: 18px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #666666;
  line-height: 22px;
}
.more {
  display: flex;
  flex-direction: row-reverse;
}
.con {
  width: 501px;
  /* height: 234px; */
  font-size: 14px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #666666;
  line-height: 22px;
  text-indent: 2em;
}
.company {
  /* margin-left: 30px; */
  /* width: 241px; */
  height: 22px;
  font-size: 22px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #333333;
  line-height: 22px;
}
.companyIn {
  width: 500px;
  height: 430px;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.introductoryFoot {
  width: 100%;
  display: flex;
  justify-content: space-around;
}
.introductoryHead {
  height: 70px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
}
.si {
  width: 171px;
  /* height: 13px; */
  font-size: 15px;
  font-family: Arial;
  font-weight: 400;
  color: #999999;
  line-height: 24px;
  text-align: center;
}
.size {
  width: 113px;
  height: 28px;
  font-size: 28px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #333333;
  line-height: 24px;
}
.introductory {
  width: 1200px;
  height: 600px;
  margin: auto;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-items: center;
}
</style>
