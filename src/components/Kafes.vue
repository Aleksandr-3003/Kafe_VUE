<template>
    <ul>
        <li v-on:click="dg = !dg">Джазвей</li>
            <div v-if="dg">  <MenuD/> </div>
        <li v-on:click="gb = !gb">Горячие булки</li>
             <div v-if="gb"> <MenuB/> </div>
        <li v-on:click="ve = !ve">Веранда</li>
            <div v-if="ve"><MenuV/></div>
            
        
      </ul>
</template>
<script>
import MenuD from '@/components/MenuD'
import MenuB from '@/components/MenuB'
import MenuV from '@/components/MenuV'
export default {
   
        components: {
        MenuD,
        MenuB,
        MenuV,
    },
    data:()=> {
            return{
                dg: false,
                gb: false,
                ve: false,
            }
    }
    

    
}
</script>