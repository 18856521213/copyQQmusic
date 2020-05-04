<template>
  <div class="bg">
      <Title title="精彩推荐"></Title>
      <el-carousel indicator-position="outside">
        <el-carousel-item  v-for="(item,index) in list" :key="index">
          <div class="content">
            <div  v-for="(item1,index) in item.content" :key="index">
              <img :src="item1.img" alt="">
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
      list:[
        { page:"1",
          content:[
            {img:"//y.gtimg.cn/music/common/upload/MUSIC_FOCUS/2348322.jpg?max_age=2592000"},
            {img:"//y.gtimg.cn/music/common/upload/MUSIC_FOCUS/2337177.jpg?max_age=2592000"}
          ]
        },
        { page:"2",
          content:[
            {img:"//y.gtimg.cn/music/common/upload/MUSIC_FOCUS/2345862.jpg?max_age=2592000"},
            {img:"//y.gtimg.cn/music/common/upload/MUSIC_FOCUS/2349695.jpg?max_age=2592000"}
          ]
        },
        { page:"3",
          content:[
            {img:"//y.gtimg.cn/music/common/upload/MUSIC_FOCUS/2347877.jpg?max_age=2592000"},
            {img:"//y.gtimg.cn/music/common/upload/MUSIC_FOCUS/2349006.jpg?max_age=2592000"}
          ]
        },
        { page:"4",
          content:[
            {img:"//y.gtimg.cn/music/common/upload/MUSIC_FOCUS/2343353.jpg?max_age=2592000"},
            {img:"//y.gtimg.cn/music/common/upload/MUSIC_FOCUS/2337028.jpg?max_age=2592000"}
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
.content{
  display:flex;
  justify-content: center;

}
.content div{
  width:600px;
  margin-left:20px;
}
.content img{
  width:100%;
}
.bg{
    background-color:#f6f6f6;
    padding-top:30px;
}

</style>