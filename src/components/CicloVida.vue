<template>
    <div>
        <h1>Ciclo vida</h1>
        <button @click="cambiarSaludo()">
            Mostrar saludo
        </button>
        <h2 style="background-color:white, color:red">
            {{saludo}}
        </h2>
    </div>  
</template>

<script>
export default {
    name: "CicloVida",
    data(){
        return{
            saludo: "Hoy es juernes"
        }
    },
    methods: {
        //AQUI INCLUIMOS NUESTROS METODOS PERSONALIZADOS
        cambiarSaludo(){
            //TODO VARIABLE O METODO DEBEMOS LLAMARLO CON this
            this.saludo = "Y mañana viernes !!!";
        }
    },
    mounted(){
        console.log("Component montado");
    },
    created(){
        console.log("Componente creado");

    },
    unmounted(){
        console.log("Componente destruido");
    },
    updated(){
        console.log("Componente modificiado")
    }

    
    }

</script>

<style scoped>

</style>