<script setup>

</script>


<template>
    <footer>
        <div class="footerContainer">
            <div class="sectionContainer sectionAddress">
                <!--<a href="https://www.google.com.mx/maps/place/UNY+(Universidad+Yucateca+de+Estudios+Estrat%C3%A9gicos)/@20.9896861,-89.6488406,17z/data=!3m1!4b1!4m6!3m5!1s0x8f56730f1c11dfc3:0xbe1ec3972e9b56e7!8m2!3d20.9896811!4d-89.6462657!16s%2Fg%2F11fn1wglh5?entry=ttu"><img src="/img/icon_mapa.png" alt=""></a>-->
                <a href="https://www.google.com.mx/maps/place/UNY+(Universidad+Yucateca+de+Estudios+Estrat%C3%A9gicos)/@20.9896861,-89.6488406,17z/data=!3m1!4b1!4m6!3m5!1s0x8f56730f1c11dfc3:0xbe1ec3972e9b56e7!8m2!3d20.9896811!4d-89.6462657!16s%2Fg%2F11fn1wglh5?entry=ttu">Av. Hidalgo No. 293 Local 7 entre 46 y 48 Col. Roma, 
                    Planta Alta, Mérida, Mexico</a>
            </div>
            
            <div class="sectionContainer sectionPhone">
                <!--<a href="tel:+529991082338"><img src="/img/icon_phone.png" alt=""></a>-->
                <a href="tel:+529991082338">999 108 2338</a>
            </div>
            
            <div class="sectionContainer sectionSocial">
                <!--<a href="https://www.facebook.com/universidadyucateca"><img src="/img/icon_facebook.png" alt=""></a>-->
                <a href="https://www.facebook.com/universidadyucateca">universidadyucateca</a>
            </div>
        </div>
    </footer>
</template>


<style lang="css" scoped>
    footer{
        width: 100%;
        height: auto;
        display: flex;
        align-items: center;
        justify-content: center;
        padding: 2rem;
        background-color: #5e1010ff;


        .footerContainer{
            width: 1440px;
            height: auto;
            display: grid;
            

            .sectionContainer{
                width: 100%;
    
                a{
                    font-size: 1.8rem;
                    line-height: 5rem;
                    color: white;
                }
            }


            .sectionAddress{
                grid-area: address;
            }
            .sectionAddress a::before{
                background-image: url('/img/icon_mapa.png');
            }


            .sectionPhone{
                grid-area: phone;
            }
            .sectionPhone a::before{
                background-image: url('/img/icon_phone.png');
            }


            .sectionSocial{
                grid-area: social
            }
            .sectionSocial a::before{
                background-image: url('/img/icon_facebook.png');
            }
        }
    }



    /** MOVIL */
    @media screen and (min-width: 320px){

        .footerContainer{
            grid-template: 
            "address"
            "phone"
            "social";
            row-gap: 2rem;


            .sectionContainer{
                display: flex;
                flex-direction: column;
                align-items: center;
            }

            .sectionContainer a{
                text-align: center;
                display: flex;
                flex-direction: column;
                align-items: center;
                text-decoration: none;
                color: inherit;
                position: relative;
                padding-top: 30px; /* espacio para el icono */
            }

            .sectionContainer a::before {
                content: '';
                /*display: block;
                margin: 0 auto;*/
                width:  5rem; /* tamaño del icono */
                height: 5rem; /* tamaño del icono */
                background-size: contain;
                background-repeat: no-repeat;
                margin-bottom: 6px; /* espacio entre el icono y el texto */
            }
        }
    }



    /** TABLET */
    @media screen and (min-width: 720px){

        .footerContainer{
            grid-template: 
            "address address"
            "phone social";
            row-gap: 2rem;
            justify-content: center;

            .sectionContainer{
                display: flex;
                flex-direction: column;
                align-items: center;
            }

            .sectionContainer a{
                display: flex;
                flex-direction: column;
                align-items: center;
                text-decoration: none;
                color: inherit;
                position: relative;
                padding-top: 30px; /* espacio para el icono */
            }

            .sectionContainer a::before {
                content: '';
                /*display: block;
                margin: 0 auto;*/
                width:  5rem; /* tamaño del icono */
                height: 5rem; /* tamaño del icono */
                background-size: contain;
                background-repeat: no-repeat;
                margin-bottom: 6px; /* espacio entre el icono y el texto */
            }

        }
    }



    /** PC */
    @media screen and (min-width: 1440px){

        .footerContainer{
            width: 1440px;
            display: grid;
            grid-template-areas: 
            "address phone social";
            grid-template-columns: 60% 20% 20%;           


            .sectionContainer a{
                display: flex;
                align-items: center;
                text-decoration: none;
                color: inherit;
                position: relative;
                padding-left: 7rem; /* espacio para el icono */
            }

            .sectionContainer a::before {
                content: '';
                position: absolute;
                left: 0;
                width: 5rem; /* tamaño del icono */
                height: 5rem; /* tamaño del icono */
                background-size: contain;
                background-repeat: no-repeat;
            }

        }
    }

</style>