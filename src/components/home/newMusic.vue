<template>
  <div>
    <Title title="新歌首发" :titleList="NewList"></Title>


    <el-carousel indicator-position="outside" :height="350+'px'" :autoplay="false" class="newMusic">
      <el-carousel-item v-for="(item,index) in list" :key="index">
         <div class="content" v-for="(item1,index) in item.content" :key="index">
           <div class="content-item" v-for="(item2,index) in item1.content" :key="index">
             <div class="item">
               <div class="img"><i class="el-icon-video-play icon"></i><img :src="item2.img" alt=""></div>
               <div class="title">
                 <p>{{item2.title}}</p>
                 <p class="name">{{item2.name}}</p>
               </div>
               <div class="time">
                 <p>{{item2.time}}</p>
               </div>
             </div>
             
           </div>

         </div>
      </el-carousel-item>
    </el-carousel>
  </div>
</template>
<script>
import Title from "@/components/common/Title.vue"
export default {
    data(){
      return{
        NewList:['最新','内地','港台','欧美','韩国','日本'],
        list:[
          {
              id:1,content:[
                {
                  name:"top",content:[
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000004DkPBz1u3bdr_3.jpg?max_age=2592000",
                          title:"愿",
                          name:"简易宏",
                          time:"03:42"
                        },
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000002xZGTc3kRGCU_1.jpg?max_age=2592000",
                          title:"飞翔的蒲公英",
                          name:"李克勤",
                          time:"05:09"
                        },
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000002f08DL0JoY3B_1.jpg?max_age=2592000",
                          title:"田舍探花",
                          name:"双笙",
                          time:"04:47"
                        }
                    

                  ]
                },
                {
                  name:"mid",content:[
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000004Mm0dR4ads9A_1.jpg?max_age=2592000",
                          title:"通行",
                          name:"剑仙",
                          time:"04:04"
                        },
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000000YszUw3LTyIq_1.jpg?max_age=2592000",
                          title:"小城姑娘",
                          name:"张艺兴",
                          time:"02:34"
                        },
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000000F5nJb1WG30g_1.jpg?max_age=2592000",
                          title:"愿Origin",
                          name:"胡梦周",
                          time:"03:59"
                        }
                    

                  ]
                },
                {
                  name:"bottom",content:[
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000004CsWWe0Z6gFR_1.jpg?max_age=2592000",
                          title:"漂洋过海来看你",
                          name:"梁静茹/艾怡良",
                          time:"04:43"
                        },
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000004ARL0O3SfJLn_2.jpg?max_age=2592000",
                          title:"自动打开定位系统",
                          name:"苏运莹",
                          time:"04:27"
                        },
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M0000013c3tV4GoLn9_2.jpg?max_age=2592000",
                          title:"蒙着眼睛走",
                          name:"GAI",
                          time:"03:01"
                        }
                    

                  ]
                }

              ]
          },    
          {
              id:1,content:[
                {
                  name:"top",content:[
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000004DkPBz1u3bdr_3.jpg?max_age=2592000",
                          title:"愿望",
                          name:"简易宏",
                          time:"03:42"
                        },
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000004DkPBz1u3bdr_3.jpg?max_age=2592000",
                          title:"愿望",
                          name:"简易宏",
                          time:"03:42"
                        },
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000004DkPBz1u3bdr_3.jpg?max_age=2592000",
                          title:"愿望",
                          name:"简易宏",
                          time:"03:42"
                        }
                    

                  ]
                },
                {
                  name:"top",content:[
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000004DkPBz1u3bdr_3.jpg?max_age=2592000",
                          title:"愿望",
                          name:"简易宏",
                          time:"03:42"
                        },
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000004DkPBz1u3bdr_3.jpg?max_age=2592000",
                          title:"愿望",
                          name:"简易宏",
                          time:"03:42"
                        },
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000004DkPBz1u3bdr_3.jpg?max_age=2592000",
                          title:"愿望",
                          name:"简易宏",
                          time:"03:42"
                        }
                    

                  ]
                },
                {
                  name:"top",content:[
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000004DkPBz1u3bdr_3.jpg?max_age=2592000",
                          title:"愿望",
                          name:"简易宏",
                          time:"03:42"
                        },
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000004DkPBz1u3bdr_3.jpg?max_age=2592000",
                          title:"愿望",
                          name:"简易宏",
                          time:"03:42"
                        },
                        {
                          img:"//y.gtimg.cn/music/photo_new/T002R90x90M000004DkPBz1u3bdr_3.jpg?max_age=2592000",
                          title:"愿望",
                          name:"简易宏",
                          time:"03:42"
                        }
                    

                  ]
                }

              ]
          }
   

        ]
      }
    },
    components:{
      Title
    }
}
</script> 
<style scoped>
.newMusic{
  padding-top:50px;
}
.content{
    display:flex;
    justify-content: center;
    padding-top:10px;
}
/* .content-item{
   display:flex; 
} */
.item{
  display:flex;
  border-bottom:1px solid #f6f6f6;
  margin-left:20px;
}
.title{
  padding-top:25px;
}
.title p{
  width:250px;
  margin:0;
  padding:0;
  padding-left:10px;
  /* color:#535353; */
}
.time{
  padding-top:22px;
  color:#9e9e9e;
  font-size: 13px;
}
.name{
  color:#9e9e9e;
  font-size: 13px;
}
.img{
  position: relative;
}
.icon{
  width:100%;
  height:100%;
  position: absolute;
  top:25%;
  left:25%;
  font-size: 50px;
  color:white;
  opacity:1;
  display: none;
}

.img:hover .icon{
  display: inline;
}


</style>