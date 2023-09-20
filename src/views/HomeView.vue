<script setup>
import { useStorage } from '@/composables/useStorage'

let food = useStorage('food')
let age = useStorage('age')
</script>

<template>
  <main>
    <p>
      What is your favorite food? <input type="text" v-model="food" />
    </p>
    <p>
      How old are you? <input type="number" v-model="age" />
    </p>
  </main>
</template>
