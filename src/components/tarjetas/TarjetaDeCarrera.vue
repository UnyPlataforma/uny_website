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

        img{
            width: 100%;
        }
    }


    @media screen and (min-width: 1440px) {
        .containerTarjeta{
        width: 400px;


        img{
            width: 100%;
        }
    }
        

    }

</style>