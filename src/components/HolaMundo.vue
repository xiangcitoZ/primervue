<template>
    <div>
        <h1> Mi primer componente VUE</h1>
        <h2>
            Su nombre es {{nombre}}
        </h2>
    </div>
</template>

<script>
    //IEMPRE DEBEMOS EXPORTAR EL NOMBRE DEL COMPONENTE
    //EN EL SCRIPTS
    export default {
         name:"HolaMundo" ,
         data() {
            //AQUI DENTRO DEBEMOS DEVOLVER LAS VARIABLES A UTILIZAR
            //EN EL COMPONENT
            return{
                nombre:"Alumno",
                numero: 14,
                miArray:[]
            }
         }
        }
</script>

<style scoped>
    h1{color:blue}
    @import './../assets/css/estilosvue.css'
</style>