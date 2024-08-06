<script setup>
</script>

<template>
    <div class="coverContainer">
        <h2>
            ¿Trabajas?
        </h2>
        <h3>
            Crece profesionalmente estudiando una licenciatura 
            los fines de semana en 2 años 8 meses.
        </h3>
    </div>
</template>

<style scoped>
    .coverContainer{
        width: 100vw;
        min-height: calc(100vh - 100px); /* 100px altura header */
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-bottom: 10rem;


        background-image: url("./img/portada_movil_color.png");
        background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.3)), url("/img/portada_pc.jpg");
        background-size: cover;
        background-repeat: no-repeat;
        background-position: 10% 50%;


        h2{
            width: 100%;
            text-align: center;
            font-size: 5rem;
        }

        h3{
            width: 70%;
            text-align: center;
            font-size: 2rem;
        }
    }


    @media screen and (min-width: 1440px) {
        .coverContainer{
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;

            background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url("/img/portada_pc.jpg");
            background-size: cover;
            background-repeat: no-repeat;


            h2{
                width: 100%;
                text-align: center;
                font-size: 10rem;
            }

            h3{
                width: 40%;
                text-align: center;
                font-size: 4rem;
            }
        }
          
    }
</style>