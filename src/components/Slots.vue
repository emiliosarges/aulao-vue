<template>
    <div class="componente">
        <h1>Compornente com Slots</h1>
        <button>
            <slot name="icone"></slot> 
            <slot name="texto">Botão</slot>
        </button>
    </div>
</template>