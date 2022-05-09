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
        {bludo:'пиво'},
        {bludo:'водка'},
        {bludo:'вино'},
        ]
        
     }
     },
}
</script>