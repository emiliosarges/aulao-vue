<script setup>
import PrimeiroComponente from './components/PrimeiroComponente.vue';
import ComDados from './components/ComDados.vue'
import ComDadosReativosPrimitivos from './components/ComDadosReativosPrimitivos.vue';
import ComDadosReativosNaoPrimitivos from './components/ComDadosReativosNaoPrimitivos.vue';
import DataBinding from './components/DataBindind.vue';
import ComProps from './components/ComProps.vue';

const borracha = "borracha"
const precoborracha = 2.50
</script>

<template>
  <header>Vue</header>
  <ComProps item="Apontador" :preco="1.99"/>
  <ComProps item="Caderno" v-bind:preco="10.25"/>
  <ComProps :item="borracha" :preco="precoborracha"/>
  <DataBinding/>
  <ComDadosReativosNaoPrimitivos/>
  <ComDadosReativosPrimitivos/>
  <ComDados/>
  <PrimeiroComponente/>
  
  
</template>

<style scoped>
</style>
