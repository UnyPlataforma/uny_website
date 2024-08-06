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
        margin-bottom: 10rem;


        h2{
            font-size: 3rem;
            text-align: center;
            color: #5e1010ff;
            margin-bottom: 1rem;
        }


        img{
            width: 90%;
            max-width: 500px;
            display: block;
            margin: 2rem auto;

            border-radius: 5px; /* Esquinas redondeadas */
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.5); /* Aumenta la sombra al pasar el mouse */
            background-color: #fff; /* Fondo blanco */
        }

        
        p{
            font-size: 1.8rem;
            line-height: 3rem;
            text-align: center;
            color: #5e1010ff;
            margin-bottom: 4rem;
        }

    }

</style>