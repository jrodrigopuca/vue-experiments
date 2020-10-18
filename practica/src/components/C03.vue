<!-- Componente: usar bind -->
<template>
    <div>
        Escribe un texto:
        <br/>
        <input type="text" v-model="mensaje">
        <br/>
        <label>{{mensaje}}</label>
    </div>
</template>

<script>
export default {
    name:'C03',
    data(){
        return{mensaje: ''}
    }
}
</script>