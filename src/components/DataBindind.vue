<template>
    <div class="componente">
        <h1>Componente com Data Binding</h1>
        <p>{{ valor }}</p>
        <!-- <input type="text" v-bind:value="valor"> --> <!-- somente ida! -->
       <!--  <input type="text" v-bind:value="valor" v-on:input="(e)=>valor = e.target.value"> --> <!-- ida e volta -->
        <!-- <input type="text" :value="valor" @input="(e)=>valor = e.target.value"> --> <!-- ida e volta com atalho -->
        <input type="text" v-model="valor"> <!-- melhor opcao - utilizando v-model com ida e volta-->
    </div>
</template>

<script setup>
import {ref} from "vue"
const valor = ref("Vue é muito legal!!")
</script>