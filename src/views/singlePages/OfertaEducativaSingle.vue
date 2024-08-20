<script setup>

    import TarjetaDeCarrera2 from '../../components/cards/TarjetaDeCarrera2.vue';
</script>

<template>

    <section class="banner">
        <div class="banner-content">
            <h1>Oferta Educativa</h1>
            <p>Descubre nuestras licenciaturas</p>
        </div>
    </section>
    
    <section class="intro">
        <p>Descubre nuestras licenciaturas diseñadas para formar profesionales 
                con una sólida preparación teórica y práctica. Ofrecemos programas 
                que te permitirán desarrollar tu potencial y alcanzar tus metas en 
                el campo que elijas</p>
    </section>

    <section class="lienciaturas">
        <div class="licenciatura">

            <TarjetaDeCarrera2 
               :imgBackUrl ="'/img/banners/banner_AE.jpg'"
            />
            
        </div>
    </section>

</template>


<style lang="css" scoped>


    .banner {
        background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('/img/banners/banner_singlePage_ofertaEducativa.jpg') no-repeat center center/cover;
        color: #fff;
        height: 400px;
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
    }

    .banner h1 {
        font-size: 5rem;
    }

    .banner p {
        font-size: 1.5rem;
        margin: 10px 0;
    }


    .intro{
        width: 100rem;
        display: block;
        margin: 0 auto;

        p{
            color: black;
            font-size: 2.5rem;
            text-align: center;
            margin: 2rem 0git ;
        }
    }
</style>