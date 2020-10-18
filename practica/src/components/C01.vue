<!-- Componente: pasar props -->
<template>
    <h1>{{mensaje}}</h1>
</template>

<script>
export default {
    name:'C01',
    props:{mensaje: String}
}
</script>

<style scope>
    h1{
        color:cadetblue;
    }
</style>