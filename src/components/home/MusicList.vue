<template>
  <div class="box">
    <Title title="歌单推荐" :titleList="MusicList"></Title>
    <el-carousel indicator-position="outside" >
      <el-carousel-item>
        <div class="content">
          <div v-for="(item,index) in List1" :key="index" class="box-content">
            <div class="content-img"><i class="el-icon-video-play icon"></i> <img :src="item.img" alt=""></div>
            <p class="content-title">{{item.title}}</p>
            <p class="content-count">{{item.count}}</p>
          </div>
        </div>
      </el-carousel-item>
      <el-carousel-item>
        <div class="content">
          <div v-for="(item,index) in List2" :key="index" class="box-content">
            <div class="content-img"><i class="el-icon-video-play icon"></i><img :src="item.img" alt=""></div>
            <p class="content-title">{{item.title}}</p>
            <p class="content-count">{{item.count}}</p>
          </div>
        </div>
      </el-carousel-item>
    </el-carousel>
  </div>
</template> 
<script>
import Title from "@/components/common/Title.vue"
export default {
  name:"MusicList",
  data(){
    return {
      MusicList:['为你推荐','网络歌曲','学习工作','经典','官方歌单','情歌'],
      List1:[
        {
          img:"//qpic.y.qq.com/music_cover/Z89aLA93LOSOicz0QOnMboqgLaiaFohjweglHh6JSoL8hrjOfFOC6DXw/300?n=1",
          title:"精选 | 好听到单曲循环的热歌",
          count:"播放量：26841.4万"
        },
        {
          img:"//qpic.y.qq.com/music_cover/MhQ4bJBPt3Yt5icXyBGNhyA75KH7nTYziamtcq57209ickxHveTia5c4Yg/300?n=1",
          title:"抖音评论过万超热歌曲合集",
          count:"播放量：4963.6万"
        },
        {
          img:"//qpic.y.qq.com/music_cover/Ye8xJJLS3zf0lX5xTNk0TMKNme42qQsE75ztd3h6pVy7R9bd0eu3vw/300?n=1",
          title:"快手热门背景音乐合集",
          count:"播放量：17420.4万"
        },
        {
          img:"//qpic.y.qq.com/music_cover/ZfWLEKXs0aUDM9Rl8E4k7CzIGeF28O602XtuKmZtcD5S2NzffacicOA/300?n=1",
          title:"经典老歌 | 免费下载重温好旋律",
          count:"播放量：3535.5万"
        },
        {
          img:"//qpic.y.qq.com/music_cover/wEXxTcWOqGq4o7ia3XxBicoMuYibWRy3uicndAYINqptTGtaNHNriarXNvg/300?n=1",
          title:"劲爆嗨曲中文dj舞曲",
          count:"播放量：2924.2万"
        }
      ],
      List2:[
        {
          img:"//qpic.y.qq.com/music_cover/amD8XDvFG8ClIJ5Hib0U0jflDmGAkNV1vqDWf3S07wto59RNZhuKdjg/300?n=1",
          title:"「忘原唱系列」惊艳耳际，一秒倾心",
          count:"播放量：3859.8万"
        },
        {
          img:"//qpic.y.qq.com/music_cover/gaSSCRswoq7NlpHA8vK1PhEKjEedic69tMicrTRXCxamBeHhVmDujLmQ/300?n=1",
          title:"周杰伦：这世界需要我的歌",
          count:"播放量：18956.5万"
        },
        {
          img:"//qpic.y.qq.com/music_cover/8KfvDey9cibtZ5xkWxRic6vtgScu1rJ2j96RMbHicskCxy7jTxB0VynZQ/300?n=1",
          title:"青春记忆 | 90后校园岁月的流行歌曲",
          count:"播放量：21422.5万"
        },
        {
          img:"//qpic.y.qq.com/music_cover/Z7haT1p6eeic63oTvdlNb7xoHMYjBDlQict0ccSicdRpgLTicqoLHqtf9g/300?n=1",
          title:"全民K歌翻唱热歌榜盘点",
          count:"播放量：20120.8万"
        },
        {
          img:"//qpic.y.qq.com/music_cover/8qyhchl8p1qt9Wib8vhcwVImibBaCpEh5TGDguU19JjnZbKbibdZk3xMA/300?n=1",
          title:"人气爆棚！一秒倾心的神仙歌曲",
          count:"播放量：393.9万"
        },
      ]
    }
  },
  components:{
    Title
  }
}
</script>
<style scoped>
.box{
  background-color:#f6f6f6;
  padding:10px 0 20px 0;
}
.box-content{
    padding:10px 10px;
}
.content{
  display:flex;
  justify-content:center;
}
.content-img{
  width:224px;
  height:224px;
  overflow: hidden;
  position: relative;
  background-color:black;
}
.content-img img{
  width:100%;
}
.content-img:hover img{
  width:110%;
  opacity:0.4;

}
.content-title{

  margin:0;
  padding:0;
  padding-top:5px;
  white-space: nowrap;
  text-overflow: ellipsis;
}
.content-count{
  margin:0;
  padding-top:10px;
  font-size: 14px;
  color:#6b6b6b;
}
.icon{
  width:100%;
  height:100%;
  position: absolute;
  top:40%;
  left:40%;
  font-size: 50px;
  color:white;
  opacity:1;
  display: none;
}
.content-img:hover .icon{
  display: inline;
}

</style>