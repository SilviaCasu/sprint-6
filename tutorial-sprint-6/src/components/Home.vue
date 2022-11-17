<template>
    <div style="homestyle">
        <h1>{{ messaggio }}</h1>
        <Escena :testos ="testos"/>
        <Boton @currentSentence = 'currentSentence'/>
       
    </div>
</template>

<script>
import Escena from './Escena.vue'
import Boton from './Boton.vue'


 export default {
  name: "Home",
  components:{
    Escena, Boton 
  },
  props:{
 messaggio: String
  
  },
  data(){
    return{
      testos: [
        {id: 0, text:"El nostre heroi estava surant per l'espai sideral quan a la llunyania va albirar una nau espacial"},
        {id: 1, text:"Sentia curiositat per l'interior de la nau i es va posar a inspeccionar-la. Va arribar "},
        {id: 2, text:"L'heroi va decidir travessar la porta que el portava a casa"},
        {id: 3, text:"Mentrestant, altres herois no van tenir tanta sort en la seva elecció ..."}
       ]
         }   
    },

    methods: {
     currentSentence: {
     
    }
  }


  
  }


</script>
    
  
<style scoped>


.homestyle{
 background-color: rgb(86, 172, 93);
  margin: 0 auto 2rem;
}



</style>
   
    
   
     
    
   
