<template>
  
  <div>
      <h2>Son</h2>
      <p>我来自父级：{{type}}</p>
      <button @click="changeType">点击修改</button>
  </div>
</template>

<script>
export default {
    name:"Son",
   data(){
       return{

       }
   },
   props:{
       type:{
           type:String,
           default:""
       },
       updataType:Function,
   },
   
   methods:{
       changeType(){
           this.updataType("success")
       }
   }

}
</script>

<style>

</style>