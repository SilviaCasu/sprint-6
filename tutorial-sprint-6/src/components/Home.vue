<template>
    <div style="homestyle">
    
        <Buttons @prevSentenceClick="prevSentenceFunction"  @nextSentenceClick="nextSentenceFunction"/>
        <Escena :testos ="testos"  :currentSentence ="currentSentence"/>
     
    </div>
</template>

<script>
import Escena from './Escena.vue'
import Buttons from './Buttons.vue'

const testos = [
        {id: 0, text:"El nostre heroi estava surant per l'espai sideral quan a la llunyania va albirar una nau espacial"},
        {id: 1, text:"Sentia curiositat per l'interior de la nau i es va posar a inspeccionar-la. Va arribar "},
        {id: 2, text:"L'heroi va decidir travessar la porta que el portava a casa"},
        {id: 3, text:"Mentrestant, altres herois no van tenir tanta sort en la seva elecció ..."}
       ];
   
let currentSentence=0;


 export default {
  name: "Home",
  components:{
    Escena,
    Buttons 
  },
  props:{
 messaggio: String,
 
  },
  data(){
    return{    
     testos, currentSentence
         } 
                  
    },

    methods: {
        prevSentenceFunction: function() {
            if (currentSentence>0) {
             this.currentSentence=currentSentence-=1
            }
        },
        nextSentenceFunction: function() {
            if (currentSentence<3) {
           this.currentSentence=currentSentence+=1
              }
        }
    }
  
  }

 

</script>
      
<style scoped>

.homestyle{
 background-color: rgb(244, 247, 245);
  
}
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  top: -10px;
}


</style>
   
    
   
     
    
   