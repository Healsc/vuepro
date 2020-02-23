<template>
    <div id="music">
        <aplayer autoplay :music="{
            title: 'Good Time',
            author: 'Owl City',
            url: 'http://www.0dutv.com/plug/down/up2.php/1511180.mp3',
            pic: 'http://www.0dutv.com/upload/magic/116.jpg',
            
        }">
        </aplayer>
        <aplayer autoplay :music="{
            title: 'Faded',
            author: '浮生若梦',
            url: 'http://www.0dutv.com/plug/down/up2.php/105030812.mp3',
            pic: 'http://www.0dutv.com/upload/magic/206.jpg',
            
        }">
        </aplayer>
         <aplayer autoplay :music="{
            title: '红昭愿',
            author: '音阙诗听',
            url: 'http://www.0dutv.com/plug/down/up2.php/200519549.mp3',
            pic: 'http://www.0dutv.com/upload/magic/235.jpg',
            
        }">
        </aplayer>
    </div>
</template>
<script>
  import Aplayer from 'vue-aplayer'
export default {
    components:{
        Aplayer
    },
    data(){
        return{
            refresh:{
                name:"音乐",
                activeClass:"music"
            }
        }
    },
    mounted() {
      this.$emit('changVal',this.refresh)  
    },
}
</script>
<style scoped>
   #music{
       margin-top: 1.2rem;
       margin-bottom: 1.2rem
   }
</style>