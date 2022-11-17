<template>
    <div>
        <button @click="$emit(nextSentence('hola'))">next</button>
        <button @click="$emit(previousSentence('hola'))">prev</button>

    </div>
</template>


<script>

export default {
  name: "Boton",
  props: ["next", "prev"]
  }

</script>

<style scoped>
button{
   
   
    width: 200px;
    height: 30px;
    background-color: red;
}

</style>
