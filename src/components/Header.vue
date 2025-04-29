<template>
    <header class="sticky top-0 z-10 backdrop-blur-md border-b border-gray-800 dark:text-gray-300 ease-in-out duration-400">
        <div class="container mx-auto flex justify-around md:justify-between items-center py-4 md:px-6">
            <h1 class="text-xl font-bold text-gray-900 dark:text-white">Euller Lourenço</h1>
            <nav class="hidden md:flex space-x-7">
                <a href="#about" class="nav-item">Sobre</a>
                <a href="#projects" class="nav-item">Projetos</a>
                <a href="#skills" class="nav-item">Habilidades</a>
                <a href="#education" class="nav-item">Educação</a>
                <a href="#contact" class="nav-item">Contato</a>
            </nav>
            <div class="flex items-center space-x-4">
                <button @click="toggleMode" class="ml-4 p-2 rounded-full hover:bg-gray-100 dark:hover:bg-gray-800 hover:cursor-pointer ease-in-out duration-300">
                    <Sun v-if="isDarkMode" class="h-5 w-5 text-yellow-400" />
                    <Moon v-else class="h-5 w-5 text-gray-700" />
                </button>
                <button @click="toggleMenu" class="flex md:hidden rounded text-gray-500 hover:text-gray-300 cursor-pointer ease-in-out duration-400">
                    <Menu v-if="!menuIsOpen" class="h-7 w-7" />
                    <X v-else class="h-7 w-7" />
                </button>
            </div>
        </div>
        <div class="duration-400 w-[90%] bg-gray backdrop-blur z-20 sticky" v-if="menuIsOpen">
            <nav class="transition-400">
                teste
            </nav>
        </div>
    </header>
</template>

<script setup>

import { ref } from 'vue';
import { Sun, Moon, Menu, X } from 'lucide-vue-next';

const isDarkMode = ref(true);
const menuIsOpen = ref(false);

function toggleMode() {
}

function toggleMenu() {
    menuIsOpen.value = !menuIsOpen.value;
}

</script>