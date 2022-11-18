<template>
    <div escenastyle>
    
        <ul>
            <li v-for="(testo, index) in testos" :key="index"  :class="{ active: index === currentSentence}">
              <strong>{{testo.text}}</strong> 
            </li>
            
        </ul> 
    </div> 
</template>


<script>
export default {
  name: "Escena",
  props: ["currentSentence","testos"],
 
  
}


</script>

<style scoped>
.escenastyle{
 background-color: rgb(172, 86, 126);

}
li{
    padding: 5px;
    margin: 10px;
    border: 1px solid;
    border-radius: 12px;
   
}
ul{
    list-style-type: none;
  margin: 0;
  padding: 0;
}



</style>




    
    