<script setup>
    import Boton1 from './botones/Boton1.vue';
</script>


<template>
    <div class="graduadosContainer">
        <h2>Alcanza tus meetas con nosotros</h2>

        <p>Nos sentimos muy orgullosos de nuestros graduados, 
            quienes con su perseverancia y compromiso han alcanzado una meta importante.</p>
        
        <img src="/img/graduados.jpg" alt="">
        
        <p>Ultimos graduados Generación 2020 - 2023</p>
        
        <div><Boton1 /></div>
    </div>
</template>


<style lang="css" scoped>
    .graduadosContainer{


        h2{
            font-size: 3rem;
            text-align: center;
            color: #5e1010ff;
            margin-bottom: 1rem;
        }

        img{
            width: 90%;
            display: block;
            margin: 2rem auto;

        }

        p{
            font-size: 1.8rem;
            text-align: center;
            color: #5e1010ff;
        }

    }

</style>