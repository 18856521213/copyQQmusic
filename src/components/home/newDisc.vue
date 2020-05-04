<template>
  <div class="pt">
    <Title title="新碟首发" :titleList="titleList"></Title>
    <div class="content">
      <div class="content-item" v-for="(item,index) in list" :key="index">
        <div class="item" v-for="(item1,index) in item.content" :key="index">
          <div><img :src="item1.img" alt=""></div>
          <div><p class="title">{{item1.title}}</p></div>
          <div><p class="name">{{item1.name}}</p></div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import Title from "@/components/common/Title.vue"
export default {
  data(){
    return {
      titleList:['内地','港台','欧美','韩国','日本','其他'],
      list:[
        {
          page:"top",
          content:[
            {
              img:"//y.gtimg.cn/music/photo_new/T002R300x300M000002f08DL0JoY3B_1.jpg?max_age=2592000",
              title:"田舍探花",
              name:"双笙"
            },
            {
              img:"//y.gtimg.cn/music/photo_new/T002R300x300M000004HDat31NgobA_1.jpg?max_age=2592000",
              title:"自以为情",
              name:"以冬"
            },
            {
              img:"//y.gtimg.cn/music/photo_new/T002R300x300M000001izsD72J4Bj4_1.jpg?max_age=2592000",
              title:"风月有解",
              name:"李常超"
            },
            {
              img:"//y.gtimg.cn/music/photo_new/T002R300x300M000002xU5vT2g3xzb_1.jpg?max_age=2592000",
              title:"田舍探花",
              name:"双笙"
            },
            {
              img:"//y.gtimg.cn/music/photo_new/T002R300x300M000004Mu6I03Eyq18_1.jpg?max_age=2592000",
              title:"田舍探花",
              name:"双笙"
            }
          ]
        },
        {
          page:"bottpm",
          content:[
            {
              img:"//y.gtimg.cn/music/photo_new/T002R300x300M000002Yopjc0j3cE2_1.jpg?max_age=2592000",
              title:"十三月",
              name:"陈又又"
            },
            {
              img:"//y.gtimg.cn/music/photo_new/T002R300x300M000004ChzKQ185Vfq_1.jpg?max_age=2592000",
              title:"U r Mine",
              name:"刘美麟"
            },
            {
              img:"//y.gtimg.cn/music/photo_new/T002R300x300M000002P9C7m2a2yY1_1.jpg?max_age=2592000",
              title:"王牌对王牌第五季",
              name:"王牌对王牌"
            },
            {
              img:"//y.gtimg.cn/music/photo_new/T002R300x300M000001DYAtf3NlXvp_1.jpg?max_age=2592000",
              title:"谁是被害者",
              name:"华语群星"
            },
            {
              img:"//y.gtimg.cn/music/photo_new/T002R300x300M000004PmX2k2B8GRX_1.jpg?max_age=2592000",
              title:"心猿归正",
              name:"刘世超"
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
.pt{
  padding-top:30px;
  background-color:#f8f8f8;
}
.content{
  padding-top:40px;
  
}
.content-item{
  display:flex;
  flex:2;
  flex-wrap:wrap;
  justify-content:center;
}
.item{
  margin-left:10px;
  padding-bottom:20px;
}
.item :nth-child(1){
  width:224px;
}
.item img{
  width:100%;
}
.item .title{
  font-size: 14px;
  color:#3d3d3d;
}
.item .name{
  font-size: 14px;
  color:#8a8a8a;
  margin:5px;
}
</style>