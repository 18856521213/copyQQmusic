<template>
  <div class="box">
    <div class="box-border">
      <h1>{{title}}</h1>
      <div class="title-box">
          <div v-for="(item,index) in titleList" :key="index">
            {{item}}
          </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name:"Title",
  data(){
    return{

    }
  },
  methods:{

  },
  props:{
     title:{
       type:String,
       default:"标题"
     },
     titleList:{
       type:Array,
       default:()=>[]
     }
  }
}
</script>
<style scoped>
.box{
  text-align: center;
}
.title-box{
  display: flex;
 justify-content:center;
 margin-top:20px;
}
.title-box div{
  width:120px;
}
.title-box div:hover{
  color:#31C27C;
}
.title-box :nth-child(1){
  color:#31C27C;
}
h1{
  letter-spacing:10px;
  font-weight: 550;
}
</style>