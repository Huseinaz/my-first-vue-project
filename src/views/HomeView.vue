<script setup>
import TheWelcome from '@/components/TheWelcome.vue'
import swal from 'sweetalert'

// eslint-disable-next-line no-undef
let message = $ref("Hello, World!");

setTimeout(() =>{
  message = "I Have Been Changed";
},2000);

let doSomething = () => {
  swal("doing it now");
};
</script>

<template>
  <main>
    <TheWelcome />
    <p>{{ message }}</p>
    <p>
      <input type="text" v-model="message" />
      <button @click="doSomething">CLick Me</button>
    </p>
  </main>
</template>
