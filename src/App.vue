<template>
  <div id="app">
    <down></down>
    <toBack></toBack>
    <top></top>
    <MusicList></MusicList>
    <newMusic></newMusic>
    <wonderful></wonderful>
    <newDisc></newDisc>
    <leaderboard></leaderboard>
    <bottomInfo></bottomInfo>
    <router-view/>
  </div>
</template>

<script>
import top from "@/components/top.vue"
import MusicList from "@/components/home/MusicList.vue"
import newMusic from "@/components/home/newMusic.vue"
import wonderful from "@/components/home/wonderful.vue"
import newDisc from "@/components/home/newDisc.vue"
import leaderboard from "@/components/home/leaderboard.vue"
import bottomInfo from "@/components/home/bottomInfo.vue"
import down from "@/components/common/down.vue"
import toBack from "@/components/common/toBack.vue"
export default {
  name: 'App',
  data(){
    return{

    }
  },
  components:{
    top,
    MusicList,
    newMusic,
    wonderful,
    newDisc,
    leaderboard,
    bottomInfo,
    down,
    toBack
  }
}
</script>

<style scoped>

</style>
