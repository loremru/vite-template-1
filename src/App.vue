<script setup lang="ts">
import HelloWorld from '@/components/HelloWorld.vue'
import { Ref, ref } from 'vue'
import { useEdit } from '@/useEdit'

const someText = ref('e')

someText.value = useEdit(someText)
</script>

<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld />
  {{ someText }}
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
