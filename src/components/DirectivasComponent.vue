<template>
    <div>
        <h1>Directivas VUE</h1>
        <ul v-if="series.length > 0">
            <li v-for="serie in series" :key="serie">
                {{serie}}
            </li>
        </ul>
        <label>Introduzca un número: </label>
        <input type="text" v-model="numero"/>
        <hr/>
        <h3 v-if="numero > 0" style="color:green">
            POSITIVO
        </h3>   
        <h3 v-else-if="numero < 0" style="color:red">
            NEGATIVO
        </h3>   
        <h3 v-else style="color:blue">
            CERO
        </h3>   
        <label>Nombre: </label>
        <input type="text" v-model="nombre"/><br/>
        <label>Edad: </label>
        <input type="text" v-model="edad"/>
        <h1>
            Nombre: {{nombre}}, Edad: {{edad}}
        </h1>
        <h1>
            <!-- PODEMOS DIBUJAR TODO EL CONTENIDO DE data()
            UTILIZANDO EL DOLAR  -->
            {{$data}}


        </h1>

    </div>
</template>

<script>
    export default {
        name: "DirectivasComponent",
        data(){
            return{
                numero: 0,
                nombre: "",
                edad: 0,
                series: ["Futurmana", "Suits",
                "The walking dead", "Como conoci a vuestra madre", "House"]
            }
        }
    }
</script>