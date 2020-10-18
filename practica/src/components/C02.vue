<!-- Componente: usar bind -->
<template>
    <div>
        <input type="text" v-bind:placeholder="mensaje">
    </div>
</template>

<script>
export default {
    name:'C02',
    data(){
        return{mensaje: 'Escribe'}
    }
}
</script>