<template>
    <div>
      <h1>{{ obj }}</h1>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue';
  
  const obj = ref({ fname: "Raj", lname: "Singh" });
  
  // Création de l'instance Vue
  const vm = obj;
  
  console.log(vm.value.fname);
  console.log(obj.value);
  console.log(obj.value.fname);
  
  </script>
  
  
  <style>
  #app {
    text-align: center;
    margin-top: 2rem;
  }
  
  p {
    font-size: 1.5rem;
  }
  
  @media (min-width: 1024px) {
    #app {
      margin-top: 4rem;
    }
  }
  </style>
  
