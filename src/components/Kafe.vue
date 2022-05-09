
<template>
  <div>
     <ul>
        <li v-for="kafe in kafes" :key="kafe.title">{{kafe.title}}
           <Menu/>
          </li>
      </ul>
    
  </div>
    
</template>
<script>
import Menu from '@/components/Menu'

export default {
  components:{
    Menu
  },
     
    data() {
        return{
            kafes: [
              {id: 1, title: 'Горячие булки'},
              {id: 2, title: 'Джазвей'},
              {id: 3, title: 'Веранда'},
            ]
        }
        
    },
}
</script>