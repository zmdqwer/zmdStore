<template>
  <div>
      <h1>Parent</h1>
      <Son  :type="type"  :updataType="updataType"/>
  </div>
</template>

<script>
import Son from "./Son"
export default {
    name:"Parent",
    data(){
        return{
            type:"半江瑟瑟半江红"
        }
    },
    components:{
        Son
    },
    methods:{
        updataType(newData){
            this.type=newData

        }
       
    }

}
</script>

<style>

</style>