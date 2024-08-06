<script setup>

</script>


<template>
    <div class="whatsapp-globe">
        <a href="https://wa.me/+529991082338/?text="><img src="/img/iconos/Logo_whatsapp.png" alt=""></a>
    </div>
</template>


<style scoped>

    .whatsapp-globe {
        position: fixed;
        bottom: 20px; /* Ajusta según tu preferencia */
        right: 20px; /* Ajusta según tu preferencia */
        z-index: 1000; /* Asegura que esté por encima de otros elementos */

    }
    .whatsapp-globe img {
        width: 80px; /* Ajusta el tamaño del icono */
        height: 80px; /* Ajusta el tamaño del icono */
        cursor: pointer;
    }


    @media screen and (min-width: 1439px) {
        .whatsapp-globe img {
            width: 100px; /* Ajusta el tamaño del icono */
            height: 100px; /* Ajusta el tamaño del icono */
            cursor: pointer;
        }
    }


</style>