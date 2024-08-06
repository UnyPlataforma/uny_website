<script setup>
    import { ref } from 'vue';

    const isOpen = ref(false);

    const toggleMenu = () => {
        isOpen.value = !isOpen.value;
    };
</script>


<template>
    <div>
        <div class="hamburger" @click="toggleMenu">
            <div :class="{ line: true, cross: isOpen }"></div>
            <div :class="{ line: true, cross: isOpen }"></div>
            <div :class="{ line: true, cross: isOpen }"></div>
        </div>
        <div v-if="isOpen" class="menu">
            <ul>
                <li><a href="#">Inicio</a></li>
                <li><a href="#">Oferta Educativa</a></li>
                <li><a href="#">Nuestra Escuela</a></li>
                <li><a href="#">Contacto</a></li>
            </ul>
        </div>
    </div>
  </template>
  

  
  <style scoped>
    .hamburger {
        width: 40px;
        height: 40px;
        display: flex;
        flex-direction: column;
        justify-content: space-around;
        align-items: center;
        cursor: pointer;

    }
    
    .line {
        width: 40px;
        height: 5px;
        background-color: #96823e;
        transition: all 0.3s ease-in-out;
    }
    

    .cross {
        position: absolute;
    }
    
    .line:nth-child(1).cross {
        transform: rotate(45deg);
        width: 40px;
        height: 5px;
    }
    
    .line:nth-child(2).cross {
        opacity: 0;
    }
    
    .line:nth-child(3).cross {
        transform: rotate(-45deg);
        width: 40px;
        height: 5px;
    }
    


    .menu {
        background-color: #fff;
        position: absolute;
        top: 100px;
        left: 0;
        width: 100%;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }
    
    .menu ul {
        list-style: none;
        padding: 0;
        margin: 0;
        text-align: center;
    }
    
    .menu li {
        padding: 15px 0;
        border-top: solid 1px #96823e;
    }
    
    .menu a {
        text-decoration: none;
        color: #96823e;
        font-weight: bold;
        font-size: 18px;
        transition: color 0.3s;
    }
    
    .menu a:hover {
        color: #555;
    }
  </style>
  