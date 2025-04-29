<template>
    <section class="py-20 md:py-32">
        <div class="container mx-auto px-4 flex flex-col md:flex-row items-center">
            <div class="md:w-1/2 mb-10 md:mb-0">
                <p class="text-2xl text-gray-500 dark:text-gray-300 mb-4">
                    Bem-vindo ao meu portfólio
                </p>
                <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold mb-4">
                    Desenvolvedor <br>
                    <span class="dark:text-violet-600">Full Stack</span>
                </h1>
                <p class="text-lg text-gray-600 dark:text-gray-500 mb-8">
                    Apaixonado por criar experiências digitais incríveis e soluções inovadoras.
                </p>
                <div class="flex space-x-4">
                    <a href="#projects" class="btn">
                        Ver Projetos
                    </a>
                    <div class="mx-4 flex items-center space-x-6">
                        <a href="https://www.linkedin.com/in/eullerlourenco/" class="hero-icon" target="_blank"><Linkedin /></a>
                        <a href="https://github.com/eullerlourenco/" class="hero-icon" target="_blank"><Github /></a>
                        <a href="mailto:euller.lourenco.silva@gmail.com" class="hero-icon" target="_blank"><Mail /></a>
                    </div>
                </div>
            </div>
            <div class="md:w-1/2 flex justify-center">
                <div
                    class="relative w-64 h-64 md:w-85 md:h-85 shadow-2xl shadow-violet-700/30 border-9 border-l-violet-950 border-t-violet-950 border-t-violet-950/75 border-r-violet-950/50 border-b-violet-950/25 rounded-full bg-emerald-100 dark:bg-emerald-900/30 overflow-hidden">
                    <img :src="photo" alt="Euller Lourenço" class="absolute inset-0 w-full h-full object-cover" />
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
import Button from '../partials/Button.vue';
import ButtonOutline from '../partials/ButtonOutline.vue';
import photo from '../../images/photo.jpg';
import { Linkedin, Github, Mail, ChevronRight, ArrowRight } from 'lucide-vue-next'



</script>