<template>
  <div class="box">
    <div>
      <div class="top-content-one">
          <div class="logo-box"><img src="../assets/logo.png" class="logo" alt=""></div>
          <div class="music-club active">音乐馆</div>
          <div class="my-music">我的音乐</div>
          <div class="client">客户端
            <div class="client-box">
              <div> <i class="el-icon-success" style="color:#31C27C"></i>HQ高品质 全员开启</div>
              <div><i class="el-icon-success" style="color:#31C27C"></i>独家音效 全面升级</div>
              <div><i class="el-icon-success" style="color:#31C27C"></i>轻盈视觉 动态皮肤</div>
              <div id="down">下载体验</div>
            </div>  
          </div> 
          <div class="open-PF">开放平台</div>
          <div class="vip">VIP</div>
          <div><el-input placeholder="请输入内容"></el-input></div>
          <div class="login">登录</div>
          <div class="open-green"><el-button type="success">开通绿钻豪华版</el-button></div>
          <div calss="give-money"><el-button>开通付费包</el-button></div>
      </div>
      <div class="top-content-two">
          <ul>
            <li>首页</li>
            <li>歌手</li>
            <li>新碟</li>
            <li>排行榜</li>
            <li>分类歌单</li>
            <li>电台</li>
            <li>MV</li>
            <li>数字专辑</li>
            <li>票务</li>
          </ul>

      </div>
    </div>
  </div>
</template>
  
<script>
export default {
  name:"top",
  data(){
    return{
        visible: false
    }
  }
}
</script>
<style scoped>
.box{
  width:100%;
  height:150px;
  display:flex;
  justify-content:center;
}
.top-content-one{
  display:flex;
  flex:1;
  height:100px;
  border-bottom:1px solid #f6f6f6;
}
.top-content-one div{
  text-align:center;
  line-height:100px;
}
.logo-box{
  width:220px;
}
.music-club,.my-music,.client,.open-PF{
  width:100px;
  cursor: pointer;
} 
.vip,.login{
  width:80px;
  cursor: pointer;
}
.music-club:hover,.my-music:hover,.client:hover,.open-PF:hover,.vip:hover,.login:hover{
  color:#31C27C;
}
.open-green{
  padding-right:10px;
}
.logo{
  padding-top:25px;
}
.el-button--success{
  background-color:#31C27C;
}
.el-button--success:hover{
  background-color:rgb(43, 175, 111);
}
.el-button{
  border-radius: 0;
}
.active{
  background-color:#31C27C;
  color:white;
}
.active:hover{
  color:white;
}
.client{
  position: relative;
}
.client .client-box{
  display: none;
  position:absolute;
  width:150px;
  border:1px solid #f6f6f6;
  top:63px;
  box-shadow:0px 0px 5px #dbdbdb;
  border-radius: 5px;;
  z-index:5;
  text-align:center;
  padding:10px 0 10px 0;
  background-color:white;
}
.client:hover .client-box{
  display: inline;
}
.client .client-box div{
  height:30px;
  line-height:30px;
  font-size: 12px;
  color:#000;
}
#down{
  border-radius: 50px;
  background-color:#31C27C;
  width:120px;
  height:25px;
  line-height:25px;
  color:white;
  margin-left:12px;

}
#down:hover{
  background-color:rgb(35, 155, 97);
}

.top-content-two {
  text-align:center;
}
.top-content-two li{
  float: left;
  width:120px;
  list-style:none;
  font-size: 15px;
}
.top-content-two li:hover{
  color:#31C27C;

}

</style>