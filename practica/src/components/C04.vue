<!-- Componente: usar bind -->
<template>
    <div>
        <input type="email" list="email-list" v-model="entrada">
        <datalist id="email-list">
            <template v-if="entrada!='' && !validarEmail()">
                <option>{{entrada}}@gmail.com</option>
                <option>{{entrada}}@hotmail.com </option>
                <option>{{entrada}}@yahoo.com </option>
            </template>
        </datalist>
    </div>
</template>

<script>
export default {
    name:'C04',
    data(){
        return{entrada: ''}
    },
    methods:{
        validarEmail: function (){
            const email=this.entrada;
            const rex = /^[a-zA-Z0-9.!#$%&'*+/=?^_`{|}~-]+@[a-zA-Z0-9-]+(?:\.[a-zA-Z0-9-]+)*$/;
            return rex.test(String(email).toLowerCase());
        },
    }
}
</script>