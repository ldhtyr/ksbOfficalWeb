<template>
  <div>
    <div class="head ">
      <div class="headContent">
        <div>
          <img src="../assets/img/logo.png" alt="" />
        </div>
        <div
          class="headIntroduce"
          @click="jumpPage(item, index)"
          v-for="(item, index) in headContent"
          :key="index"
        >
          <div :style="headContentJudge == index ? 'color: #ff3a2f' : ''">
            {{ item }}
          </div>
          <div
            :style="
              headContentJudge == index
                ? 'width: 100%;height: 2px; background: #ff3a2f'
                : ''
            "
          ></div>
        </div>
      </div>
    </div>
    <div>
      <div v-if="headContentJudge == 0">
        <PageJu></PageJu>
      </div>
      <div v-if="headContentJudge == 1">
        <AboutUs></AboutUs>
      </div>
      <div v-if="headContentJudge == 2">
        <ProductCenter></ProductCenter>
      </div>
      <div v-if="headContentJudge == 3">
        <News></News>
      </div>
      <div v-if="headContentJudge == 4">
        <Connect></Connect>
      </div>
    </div>
    <div class="footer">
      <div class="footerContent">
        <div class="one">
          <div class="phone">联系方式</div>
          <div class="content">
            <div>销售部电话：86-10-87227898</div>
            <div>
              商务部电话：86-10-87227898
            </div>
            <div>邮箱：Service@kseiburg.com</div>
          </div>
        </div>
        <div class="one">
          <div class="phone">关于我们</div>
          <div class="content">
            <div>企业简介</div>
            <div>经典案例</div>
            <div>企业规模</div>
          </div>
        </div>
        <div class="one">
          <div class="phone">产品中心</div>
          <div class="content">
            <div>主控模块</div>
            <div>感知模块</div>
            <div>霍尔传感器</div>
            <div>显示屏</div>
          </div>
        </div>
        <div class="one">
          <div class="phone">新闻中心</div>
          <div class="content">
            <div>新闻动态</div>
          </div>
        </div>
        <div class="one">
          <img
            style="width:183px;height:57px"
            src="../assets/img/homePage_loge.png"
            alt=""
          />
          <div class="company">北京凯思博科技有限公司</div>
        </div>
      </div>
      <div class="ma">
        公司统一社会信用代码：91110107766787206A | CopyRight授权所有
        京ICP备07503795号-1 | 京公网安备1101070200175号FAX: 010-68654980
      </div>
      <div class="adress">地址：北京市大兴区科创十三街德为科技园</div>
    </div>
  </div>
</template>

<script>
import PageJu from "./PageJu.vue";
import ProductCenter from "./ProductCenter.vue";
import AboutUs from "./AboutUs/AboutUs.vue";
import Connect from "./Connect/Connect.vue";
import News from "./News/News.vue";
export default {
  components: { PageJu, ProductCenter, Connect, News, AboutUs },
  data() {
    return {
      headContentJudge: 0,
      headContent: ["首 页", "关于我们", "产品中心", "新闻中心", "联系我们"],
    };
  },
  computed: {},
  watch: {},
  methods: {
    jumpPage(item, index) {
      this.headContentJudge = index;
    },
  },

  created() {},

  mounted() {},
  props: [],
  beforeCreate() {},
  updated() {},
};
</script>
<style scoped>
.middle {
  width: 1903px;
}
.adress {
  width: 300px;

  font-size: 14px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #dddddd;
  line-height: 27px;
  margin: auto;
}
.ma {
  width: 997px;
  height: 15px;
  font-size: 14px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #dddddd;
  margin: auto;
}
.company {
  width: 197px;
  /* height: 17px; */
  font-size: 17px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #dddddd;
  line-height: 27px;
}
.content {
  width: 255px;
  height: 73px;
  font-size: 18px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #dddddd;
  line-height: 27px;
}
.phone {
  width: 96px;
  height: 24px;
  font-size: 24px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #f1f1f1;
}
.one {
  height: 200px;
  display: flex;
  flex-direction: column;
  /* align-items: center; */
  justify-content: space-around;
}
.footerContent {
  width: 1300px;
  height: 233px;
  margin: auto;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.footer {
  width: 1903px;
  height: 543px;
  background: #333333;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}
.headIntroduce {
  height: 50px;
  display: flex;
  flex-direction: column;
  font-weight: 400;
  justify-content: space-around;
}
.headContent {
  width: 1200px;
  height: 100%;
  margin: auto;
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.head {
  width: 1903px;
  height: 80px;
}
</style>
