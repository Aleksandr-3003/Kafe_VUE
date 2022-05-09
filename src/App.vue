<template>
  <div id="app">
    
    <h1>Hello</h1>

    <hr/>
    
    
    <button v-on:click="sh = !sh">{{sh?'СКРЫТЬ':'показать'}} список</button>
    
    <div v-if="sh">
         
       <Kafes/> 
     
    </div>
    
    <hr>
    
    

   
  </div>
</template>
<script>
import Kafes from '@/components/Kafes'
import MenuD from '@/components/MenuD'
import MenuB from '@/components/MenuB'
import MenuV from '@/components/MenuV'



export default {
  
  components: {
     Kafes,
     MenuD,
     MenuB,
     MenuV,
    
  },
  data:() => {
    return{
    awe: false,
    sh: false,
    
  }}
}

</script>
<style>


</style>

