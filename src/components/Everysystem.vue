<template>
  <div class="home">
    <p>各系统接入表数量</p>
    <div class="menu">
      <el-carousel
        background-color="#f5f7fd"
        indicator-position="none"
        :interval="5000"
        arrow="always"
        height="540px"
      >
        <el-carousel-item v-for="item in 4" :key="item.id">
          <ul>
            <li v-for="item in 5"><SystemVue></SystemVue></li>
            <li v-for="item in 5"><SystemVue></SystemVue></li>
            <li v-for="item in 5"><SystemVue></SystemVue></li>
          </ul>
        </el-carousel-item>
      </el-carousel>
    </div>
  </div>
</template>

<script>
import SystemVue from "./System.vue";
import { reactive } from "vue";

export default {
  name: "Everysystem",
  components: { SystemVue },
  setup() {
    let list = reactive([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14]);
    return {
      list,
    };
  },
};
</script>
<style scoped lang="less">
.home {
  position: relative;
  padding: 0;
  margin: 0;
  background-color: #fdffff;
  border: 1px, solid red;
  padding-left: 40px;
}
p {
  font-size: 20px;
  margin: 15px 0px;
  font-weight: bold;
}
.menu {
  width: 100%;
  height: auto;
  background-color: #f5f7fd;
}
ul li {
  list-style-type: none;
  text-decoration: none;
  text-align: center;
}
.el-carousel__item h3 {
  color: #475669;
  opacity: 0.75;
  line-height: 300px;
  margin: 0;
  text-align: center;
}
.el-carousel__item:nth-child(2n) {
  background-color: #f5f7fd;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #f5f7fd;
}
/deep/ .el-carousel__arrow {
  font-size: 20px;
  width: 40px;
  height: 40px;
  background-color: #dfe1e3;
  margin-left: -10px;
  border-radius: 0;
}
/deep/ .el-carousel__arrow :hover {
  background-color: #3467c9;
}
</style>
