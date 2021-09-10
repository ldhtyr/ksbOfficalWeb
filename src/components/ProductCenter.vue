<template>
  <div class="">
    <div>
      <div style="width:1903px;height:600px">
        <img
          style="width:1903px;height:600px"
          src="../assets/img/ProductCenter_banner.png"
          alt=""
        />
      </div>
      <div style="width:1903px">
        <div style="height:80px"></div>
        <div style="text-align:center">
          <div class="proCenter">产品中心</div>
          <div
            style="width: 1903px;
height: 2px;
background: #D4D4D4;"
          ></div>
          <div class="xian"></div>
        </div>
        <div class="name">
          <div style="height: 36px;text-align:center;line-height:36px">
            名称 :
          </div>
          <div
            @click="ProductCh(index)"
            :class="ProductChoce == index ? 'con' : 'cons'"
            v-for="(item, index) in data"
            :key="index"
          >
            {{ item.name }}
          </div>
        </div>
        <div style="margin-bottom:80px">
          <div v-for="(item, index) in data" :key="index">
            <div v-if="ProductChoce == index" class="jies">
              <img style="width:564px;height:423px" :src="item.img" alt="" />
              <div class="content">{{ item.content }}</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      ProductChoce: 0,
      data: [
        {
          name: "动态电压恢复装置",
          img: "img/ProductCenter_DVR.png",
          content:
            "动态电压恢复装置（DVR）通过实时监测电网电压情况，当监测到电压出现瞬降或浪涌后，调节装置能够迅速将后端设备的供电切换到由瞬态电压调节装置供电。凯思博推出的PowerSuite-DVR动态电压恢复装置，具备快速响应，精确补偿，无缝退出的卓越性能，功率高达2000KVA，是治理电压扰动的最可靠的解决方案，也是目前最先进、最可行、性价比最高的电压扰动治理技术。",
        },
        { name: "有源滤波器" },
        { name: "静止无功发生器" },
        { name: "感知单元" },
        { name: "主控单元" },
        { name: "锂电池储能柜" },
        { name: "分布式锂电池UPS" },
      ],
    };
  },
  computed: {},
  watch: {},
  methods: {
    ProductCh(index) {
      this.ProductChoce = index;
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
.content {
  width: 563px;
  display: flex;
  align-items: center;
  color: #666666;
  font-size: 18px;
}
.jies {
  width: 1200px;
  height: 423px;
  margin: auto;
  display: flex;
  justify-content: space-around;
}
.con {
  width: 150px;
  height: 36px;
  background: #ff3a2f;
  text-align: center;
  line-height: 36px;
  border: 1px solid #ff3a2f;
  color: #fff;
}
.cons {
  width: 150px;
  height: 36px;
  background: #fff;
  text-align: center;
  line-height: 36px;
  border: 1px solid #ccc;
}
.name {
  width: 1200px;
  height: 100px;

  margin: auto;
  margin-top: 50px;
  display: flex;
  justify-content: space-around;
}
.xian {
  width: 118px;
  height: 2px;
  background: #ff3a2f;
  position: absolute;
  left: 890px;
  top: 784px;
}
.proCenter {
  width: 99px;
  height: 24px;
  font-size: 24px;
  font-family: Microsoft YaHei;
  font-weight: 400;
  color: #ff3a2f;
  line-height: 20px;
  margin: auto;
}
</style>
