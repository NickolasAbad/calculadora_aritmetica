<script setup>
    import Header from './components/Header.vue'
    import Calculator from './components/Calculator.vue'
    import Result from './components/Result.vue'
    import { getOperacao, estado } from './scripts/Scripts.vue'
</script>

<template>
  <Header />
  <Calculator :estado="estado"/>
  <Result :estado="estado" :operacao="getOperacao()"/>
</template>

<style scoped>
</style>
