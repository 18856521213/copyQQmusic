<template>
  <div class="box">
    <div class="img"><img src="@/assets/logo.png" alt=""></div>
    <div class="box-font">千万高品质曲库尽享</div>
    <el-button  class="button"><i class="el-icon-s-platform icon"></i> 客户端下载</el-button>
  </div>
</template>
<script>
export default {
  
}
</script>
<style scoped>
.box{
  position: fixed;
  top:170px;
  right:50px;
  border-radius: 3px;
  box-shadow: #eeeeee 0px 2px 5px;
  padding:10px 10px;
  text-align: center;
  background-color:white;
  z-index: 99;
}

.img img{
  width:130px;
}
.box-font{
  color:#7f7f7f;
  font-size: 17px;
  padding:15px 0;
}
.button{
  background-color:#31c27c;
  color:#fff;
  border-radius: 20px;
  height:30px;
  width:150px;
    margin:0;
  padding: 0;
}
.button:hover{
  background-color:#2caf6f;
}

.icon{
  font-size:20px;
}
</style>