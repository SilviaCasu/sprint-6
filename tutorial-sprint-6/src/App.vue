
<template>

  <div class="appstyle">
   <Home messaggio="App è il componente principale"/>
 </div>
</template>


<script>

import Home from './components/Home.vue'
export default {
  name: 'App',
  components:{
    Home
  }
  
}

</script>





<style scoped>


.appstyle{
 background-color: white;
  margin: 0 auto 2rem;
}



</style>
