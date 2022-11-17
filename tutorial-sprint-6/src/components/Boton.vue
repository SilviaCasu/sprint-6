<template>
    <div>
        <button @click="$emit(currentSentence('hola'))">prev</button> <!-- provando -->
        <button @click="$emit(currentSentence)">next</button>
       

    </div>
</template>


<script>

export default {
  name: "Boton",
  props: ["currentSentence"]
  }

</script>

<style scoped>
button{
   
   
    width: 200px;
    height: 30px;
    background-color: red;
}

</style>
