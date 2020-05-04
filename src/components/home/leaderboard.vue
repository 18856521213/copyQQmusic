<template>
  <div class="box">
    <Title title="排行榜"></Title>
    <div class="content">
      <div class="item hot" @mouseout="changeIcon">
        <div class="top">
          <div>{{list.hot.title}}</div>
          <h1>{{list.hot.name}}</h1>
          <div class="icon">
            <i class="el-icon-minus" v-show="line"></i>
            <i class="el-icon-video-play" v-show="play"></i>
          </div>
        </div>
        <ul>
          <li v-for="(item,index) in list.hot.music" :key="index">
            <div>{{item.id}}.</div>
            <div>{{item.musicName}}</div>
            <div>{{item.name}}</div>
          </li>
        </ul>
      </div>
      <div class="item new" @mouseout="changeIcon">
        <div class="top">
          <div>{{list.new.title}}</div>
          <h1>{{list.new.name}}</h1>
          <div class="icon">
            <i class="el-icon-minus" v-show="line"></i>
            <i class="el-icon-video-play" v-show="play"></i>
          </div>
        </div>
        <ul>
          <li v-for="(item,index) in list.hot.music" :key="index">
            <div>{{item.id}}.</div>
            <div>{{item.musicName}}</div>
            <div>{{item.name}}</div>
          </li>
        </ul>
      </div>
      <div class="item popur" @mouseout="changeIcon">
        <div class="top">
          <div>{{list.popur.title}}</div>
          <h1>{{list.popur.name}}</h1>
          <div class="icon">
            <i class="el-icon-minus" v-show="line"></i>
            <i class="el-icon-video-play" v-show="play"></i>
          </div>
        </div>
        <ul>
          <li v-for="(item,index) in list.popur.music" :key="index">
            <div>{{item.id}}.</div>
            <div>{{item.musicName}}</div>
            <div>{{item.name}}</div>
          </li>
        </ul>
      </div>
      <div class="item EA" @mouseout="changeIcon">
        <div class="top">
          <div>{{list.EA.title}}</div>
          <h1>{{list.EA.name}}</h1>
          <div class="icon">
            <i class="el-icon-minus" v-show="line"></i>
            <i class="el-icon-video-play" v-show="play"></i>
          </div>
        </div>
        <ul>
          <li v-for="(item,index) in list.EA.music" :key="index">
            <div>{{item.id}}.</div>
            <div>{{item.musicName}}</div>
            <div>{{item.name}}</div>
          </li>
        </ul>
      </div>
      <div class="item Korea" @mouseout="changeIcon">
        <div class="top">
          <div>{{list.Korea.title}}</div>
          <h1>{{list.Korea.name}}</h1>
          <div class="icon">
            <i class="el-icon-minus" v-show="line"></i>
            <i class="el-icon-video-play" v-show="play"></i>
          </div>
        </div>
        <ul>
          <li v-for="(item,index) in list.Korea.music" :key="index">
            <div>{{item.id}}.</div>
            <div>{{item.musicName}}</div>
            <div>{{item.name}}</div>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>
<script>
import Title from "@/components/common/Title.vue"
export default {
  data(){
    return {
      line:true,
      play:false,
      list:{
        hot:{title:"巅峰榜",name:"热歌",music:[{id:1,musicName:"点歌的人",name:"海来阿木"},{id:2,musicName:"少年",name:"梦然"},{id:3,musicName:"后来遇到他",name:"胡66"}]},
        new:{title:"巅峰榜",name:"新歌",music:[{id:1,musicName:"夏天的风",name:"Uu"},{id:2,musicName:"光点",name:"肖战"},{id:3,musicName:"纸船",name:"薛之谦/郁可唯"}]},
        popur:{title:"巅峰榜",name:"流行指数",music:[{id:1,musicName:"夏天的风",name:"蓝心羽"},{id:2,musicName:"爱人啊",name:"张杰"},{id:3,musicName:"你真的很特别",name:"杜海涛"}]},
        EA:{title:"巅峰榜",name:"欧美",music:[{id:1,musicName:"Salt",name:"Ava Max"},{id:2,musicName:"I Hope",name:"Gabby Barrett"},{id:3,musicName:"You know I'll",name:"DJ Haning"}]},
        Korea:{title:"巅峰榜",name:"韩国",music:[{id:1,musicName:"Saty Tonight",name:"金请夏"},{id:2,musicName:"Nonstop",name:"OH MY"},{id:3,musicName:"Refresh",name:"Zico"}]}
      }
      
    }
  },
  methods:{
    changeIcon(){
      this.line=!this.line
      this.play=!this.play
      
    }
  },
  components:{
    Title
  }  
}
</script>
<style scoped>
.box{
  padding:30px 0;

}
.top{
  text-align: center;
}
.top:nth-child(1){
  font-size: 18px;
}
.top h1{
  margin:10px 0;
}
.content{
  display:flex;
  justify-content:center;
}
.item{
  width:300px;
  padding:20px 0px;
  margin-right:10px;
  width:230px;
  color:#ffffff;
}
.item li{
  list-style: none;
  padding:15px 0;
}
.hot{
  background-color:#cf728a;
}
.new{
  background-color:#6d96b1;
}
.popur{
  background-color:#6cbeb2;
}
.EA{
  background-color:#538f94;
}
.Korea{
  background-color:#e99c6f;
}
.icon{
  font-size: 50px;;
}
</style>