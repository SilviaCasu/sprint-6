<template>
    <button @click="$emit('prevSentenceClick')">prev</button> 
    <button @click="$emit('nextSentenceClick') ">next</button> 
</template>

<style>
button{
    margin: 5px; 
    min-width: 290px;
    height: 40px;
    background-color: rgb(236, 231, 231);
    border: 1px solid;
    border-color: rgb(44, 41, 41);
    }
    .active {
        background-color: rgb(250, 209, 209);
        border:1px solid rgb(110, 106, 106);
}

</style>