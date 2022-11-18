<template>
  <div class="system">
    <div class="box">LP</div>
    <div class="content">
      <p class="big">40</p>
      <p class="small">Leads Pipeline</p>
    </div>
  </div>
</template>
<script>
export default {
  name: "System",
};
</script>

<style scoped>
.system {
  width: 210px;
  height: 150px;
  background-color: #fdffff;
  float: left;
  margin: 10px 14px 10px 20px;
}
.box {
  width: 60px;
  height: 60px;
  margin-left: 20px;
  background-color: #3668cd;
  text-align: center;
  line-height: 60px;
  border-radius: 50%;
  color: #c7d9fc;
  font-size: 14px;
  float: left;
  margin-top: 40px;
}
.content {
  position: relative;
  float: left;
}
.big {
  position: absolute;
  font-size: 20px;
  margin: 40px 0 27px 13px;
}
.small {
  position: absolute;
  font-size: 10px;
  color: #78787a;
  margin-top: 80px;
  margin-left: 13px;
  white-space: nowrap;
}
</style>
