<template>
  <div class="main1">

      <div class="bg">
                <el-button class="button" circle><el-avatar :size="100" :src="circleUrl"></el-avatar></el-button>
                <h1 style="margin-right: 150px; color: black;">小熊软糖杀手</h1>        
            </div>
            
     
  </div>
</template>

<script>
export default {
  name: "Main1",
  data() {
        return {
            circleUrl: require("../../assets/block.png"),//头像图片
        }
    },
}
</script>

<style scoped>
.main1 {
  width: 100%;
  height: 900px;
  /* background-color: red; */

}

.bg {
  width: 100%;
  height: 100%;
  margin-left: 50px;
  background: url('../../assets/bg.gif');
  /* background-size: cover; */
}
.button {
    margin-top: 20px;
    margin-right: 150px;
    background: linear-gradient(to bottom, #8da1f8, #fab2f1);
}
</style>
