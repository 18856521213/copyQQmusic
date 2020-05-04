<template>
  <div class="box">
    <el-backtop :bottom="123" :right="70">
      <div class="item"><i class="el-icon-arrow-up"></i> </div>
    </el-backtop>
    <div class="item content">反馈</div>
    <div class="item"><i class="el-icon-document icon"></i> </div>
  </div>
</template>
<script>
export default {
  
}
</script>
<style scoped>
.box{
  position: fixed;
  bottom: 30px;
  right:70px;
  z-index: 3;
  cursor: pointer;
}
.item{
  width:38px;
  height:40px;
  border:1px solid rgb(194, 194, 194);
  background-color: white;
  margin-bottom:3px;
  text-align: center;
  line-height:40px;
}
.icon{
  font-size: 20px;

}
.el-backtop{
  color:#000;
}
.content{
  font-size: 14px;
}
.content:hover{
  color:#31c27c;
}
</style>