<script setup>
    import MenuMovil from "./MenuMovil.vue"
</script>


<template>
    <header>

        <!-- Area Logo -->
        <div class="areaLogo">
            <img src="/img/Logo_UNY.png" alt="Logo Uny">
        </div>


        <!-- Area menuButton-->
        <div class="areaMenuButton">
            <MenuMovil />
        </div>
    
    </header>
</template>


<style lang="css" scoped>

    header {
        display: flex;
        width: 100%;
        height: 100px;
        padding: 1rem 2rem;
        box-sizing: border-box;
        background-color: white;

    
        .areaLogo{
            display: flex;
            align-items: center;
            width: 50%;
            height: 100%;

            img{
                width: 80px;
                height: 80px; 
            }
        }

        .areaMenuButton{
            width: 50%;
            height: 100%;
            display: flex;
            align-items: center;
            justify-content: right;
        }
    }
</style>