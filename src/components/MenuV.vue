<template>
    <ol>
        <li v-for="mbuls in mbul" :key="mbuls.bludo">{{mbuls.bludo}}
          </li>
      
    </ol>
</template>
<script>
export default {
    
    data(){
    return {
        mbul:[
        {bludo:'паста'},
        {bludo:'хачапури'},
        {bludo:'пильмени'},
        ],        
     }
     },
}
</script>