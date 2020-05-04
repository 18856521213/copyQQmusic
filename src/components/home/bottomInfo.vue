<template>
<div class="box">
  <div class="content">
    <div class="item">
      <div>
        <h3>下载QQ音乐客户端</h3>
      </div>
      <div class="version">
        <div class="version-item">
          <div><i class="el-icon-s-platform icon"></i></div>
          <div>PC端</div>
        </div>
        <div class="version-item">
          <div><i class="el-icon-video-play icon"></i></div>
          <div>Mac端</div>
        </div>
        <div class="version-item">
          <div><i class="el-icon-s-opportunity icon"></i></div>
          <div>Android端</div>
        </div>
        <div class="version-item">
          <div><i class="el-icon-s-check icon"></i></div>
          <div>iphone端</div>
        </div>     
      </div>
      <div>
        <p>开放平台</p>
      </div>
      <div>
        <p class="chang-color">QQ音乐开放平台</p>
        <p class="chang-color">腾讯音乐人</p>
      </div>
    </div>
    <div class="item">
      <div>
        <h3>特色产品</h3>
      </div>
      <div class="version">
        <div class="version-item">
          <div><i class="el-icon-loading icon"></i></div>
          <div>全民K歌</div>
        </div>
        <div class="version-item">
          <div><i class="el-icon-umbrella icon"></i></div>
          <div>Super Sound</div>
        </div>
        <div class="version-item">
          <div><i class="el-icon-headset icon"></i></div>
          <div>Qplay</div>
        </div>
      </div>
      <div>
        <p class="chang-color">车载互联</p>
        <p class="chang-color">QQ演出</p>
      </div>
      <div>
        <p class="chang-color">TME集团官网</p>
        <p class="chang-color">腾讯音乐</p>
      </div>
    </div>
    <div class="item">
      <div><h3>合作连接</h3></div>
      <div class="cooperation">
        <div class="cooperation-item">
          <p>CJ ENM</p>
          <p>最新版音乐</p>
          <p>QQ浏览器</p>
          <p>企鹅FM</p>
        </div>
        <div class="cooperation-item">
          <p>腾讯视频</p>
          <p>腾讯社交广告</p>
          <p>腾讯微云</p>
          <p>智能电视网</p>
        </div>
        <div class="cooperation-item">
          <p>手机QQ空间</p>
          <p>电脑管家</p>
          <p>腾讯云</p>
          <p>当贝市场</p>
        </div>
      </div>
    </div>
  </div>
  <div class="bottom-info">
      <div class="bottom-content">
        <div>关于腾讯</div>
        <div>About Tencent</div>
        <div>服务条款</div>
        <div>用户协议条款</div>
        <div>隐私政策</div>
        <div>权利声明</div>
        <div>广告服务</div>
        <div>腾讯招聘</div>
        <div>客服中心</div>
        <div>网站导航</div>
      </div>
      <div class="canDo">
        <p>Copyright © 1998 - 2020 Tencent. <span> All Rights Reserved.</span></p>
      </div>
      <div class="company">
        <div>腾讯公腾讯网络司</div>
        <div>版权所有</div>
        <div>文化经营许可证</div>
      </div>
  </div>
</div>
</template>
<script>
export default {
  
}
</script>
<style scoped>
.box{
  background-color:#333;
  padding:60px 0;
  color:#7f7f7f;
  font-weight: 200;
  font-size: 14px;;
}
.content{
  display:flex;
  justify-content:center;
}
.item{
  margin-left:80px;
}
.version{
  display:flex;
  text-align: center;
}
.icon{
  font-size: 50px;
}
.version-item{
  margin-right:30px;
}
.version-item:hover{
  color:#31c27c;
}

.cooperation{
  display:flex;
}

.chang-color:hover{
  color:#31c27c;
}
.cooperation p:hover{
  color:#31c27c;
}
.cooperation-item{
  margin-right:20px;
}
.bottom-info{
  text-align: center;
  font-size: 12px;
}
.bottom-content{
  display:flex;
  justify-content: center;
  padding-top:50px;

}
.bottom-content div{
  padding:0px 7px;
  border-right:1px solid #7f7f7f;
}
.bottom-content div:hover{
  color:#31c27c;
}
.canDo{
  display:flex;
  justify-content:center;
}
.canDo span:hover{
  color:#31c27c;
}
.company{
  display:flex;
  justify-content: center;
}
.company div{
  margin-right:15px;
}
.company div:hover{
  color:#31c27c;
}
</style>  