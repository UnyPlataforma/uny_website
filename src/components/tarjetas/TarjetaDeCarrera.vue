<script setup>
    import { defineProps } from 'vue';

    const props = defineProps({
        imageUrl: {
            type: String,
            required: true,
        }
    });

</script>


<template>
    <div class="containerTarjeta">
        <img :src="imageUrl" alt="">
    </div>
</template>


<style lang="css" scoped>

    .containerTarjeta{
        width: 280px;

        border: 1px solid #ccc; /* Borde sólido de 1px con color gris claro */
        border-radius: 5px; /* Esquinas redondeadas */
        padding: 20px; /* Espacio interno */
        box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1); /* Sombra sutil */
        background-color: #fff; /* Fondo blanco */
        transition: transform 0.3s ease, box-shadow 0.3s ease; /* Transición suave para transformación y sombra */

        img{
            width: 100%;
        }
    }


    .containerTarjeta:hover {
        transform: scale(1.05); /* Aumenta el tamaño al pasar el mouse */
        box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2); /* Aumenta la sombra al pasar el mouse */
    }


    @media screen and (min-width: 1440px) {
        .containerTarjeta{

        img{
            width: 100%;
        }
    }
        

    }

</style>