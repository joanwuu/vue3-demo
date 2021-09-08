<template>
  <div>
    <h1>login page</h1>
    <el-button @click="goHome">go home</el-button>
  </div>
</template>

<script setup>
import { reactive } from 'vue'
import { useRouter } from 'vue-router'

const state = reactive({count: 0});
const router = useRouter();
const goHome = () => {
  console.log('gogogo')
  router.push('/welcome');
}
</script>

<style scoped>
a {
  color: #42b983;
}
</style>
