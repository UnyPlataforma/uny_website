<script setup>
    import TarjetaDeCarrera from './tarjetas/TarjetaDeCarrera.vue';
</script>
    
<template>

    <div class="carrerasContainer">

        <div class="tarjetasContainer">

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

            <TarjetaDeCarrera 
                :imageUrl="'/img/tarjetaAR.jpg'"
            />

        </div>
    </div>
    
</template>

<style lang="css" scoped>
    .carrerasContainer{
        width: 100%;
        display: flex;
        justify-content: center;
        margin-bottom: 10rem;
    }

    .tarjetasContainer{
        max-width: 1440px;
        height: auto;
        display: flex;
        justify-content: center;
        row-gap: 5rem;
        column-gap: 10rem;
        flex-wrap: wrap;
    }


</style>