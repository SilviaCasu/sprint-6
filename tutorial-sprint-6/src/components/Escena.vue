<template>
    <div escenastyle>
        <ul>
            <li v-for="testo in testos" :key="testo.id"> <strong>{{testo.text}}</strong>  </li>
            
        </ul>
    </div>
</template>


<script>

export default {
  name: "Escena",
  props: ["testos", "currentSentence"]
  }

</script>

<style scoped>
.escenastyle{
 background-color: rgb(172, 86, 126);
  margin: 0 auto 2rem;
}
li{
    padding: 5px;
    margin: 10px;
    border: 1px solid;
    border-radius: 12px;
}


</style>




    
    