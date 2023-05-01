<template>
  <main>
    <div>
    <h4>
      Current count: 
    </h4>
    <h1>{{ count }}</h1>
    <button @click="count--">-</button>
    <button @click="count++">+</button>
  </div>
  </main>
</template>

<script setup>
import {ref} from "vue";

const count = ref(0);
</script>

<style scoped>
main{
  background-color: rgb(63, 63, 63);
  height: 100vh;
  width: 100vw;
  color: rgb(228, 228, 228);
  display: flex;
  align-items: center;
  justify-content: center;

}
div{
  text-align: center;
}

button{
  margin: 5%;
  width: 30px;

}
</style>