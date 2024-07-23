<script setup>
    import TarjetaDeCarrera from './tarjetas/TarjetaDeCarrera.vue';
</script>
    
<template>
    <div class="container">

        <TarjetaDeCarrera 
            :imageUrl="'/img/tarjetaAR.jpg'"
        />

        <TarjetaDeCarrera 
            :imageUrl="'/img/tarjetaAE.jpg'"
        />

        <TarjetaDeCarrera 
            :imageUrl="'/img/tarjetaCP.jpg'"
        />

        <TarjetaDeCarrera 
            :imageUrl="'/img/tarjetaAE.jpg'"
        />

        <TarjetaDeCarrera 
            :imageUrl="'/img/tarjetaCP.jpg'"
        />



    </div>
</template>

<style lang="css" scoped>
    .container{
        width: 100%;
        height: auto;
        display: flex;
        justify-content: center;
        row-gap: 5rem;
        column-gap: 5rem;
        flex-wrap: wrap;
        margin-bottom: 5rem;


        .cuadro{
            width: 300px;
            height: 300px;
            background-color: aqua;
        }
    }


</style>