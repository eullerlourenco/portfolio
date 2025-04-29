<template>
    <section class="py-16 md:py-18">
        <div class="container mx-auto px-4 flex flex-col md:flex-row items-center">
            <div class="md:w-4/7 mb-10 md:mb-0">
                <div class="bg-linear-to-r from-gray-900 pb-1 mb-6"></div>
                <h1 class="text-4xl font-bold my-4 mb-12">
                    <span class="font-normal text-violet-900 font-mono"><</span> 
                    Sobre mim 
                    <span class="font-normal text-violet-900 font-monp">/></span>
                </h1>
                <p class="text-lg text-gray-600 dark:text-gray-400 mb-5">
                    Sou um Desenvolvedor Full Stack e atualmente curso Desenvolvimento de Software Multiplataforma.
                    Tenho
                    uma base sólida em desenvolvimento, com uma paixão especial por Desenvolvimento Web.
                </p>
                <p class="text-lg text-gray-600 dark:text-gray-400 mb-5">
                    Gosto de enfrentar novos desafios, estou sempre em busca de aprendizado contínuo e me adapto
                    facilmente a
                    novas tecnologias. No momento, trabalho em projetos freelancers e pessoais, além de me aprofundar
                    nos estudos de desenvolvimento para aprimorar ainda mais minhas habilidades.
                </p>
            </div>
            <div class="md:w-3/7 md:mx-8 mb-10 md:mb-0 flex flex-col justify-center items-center py-8">
                <h1 class="text-center font-bold text-3xl my-4 mb-8 text-gray-900 dark:text-gray-200">
                    Baixe meu currículo
                </h1>
                <p class="text-center text-lg text-gray-600 dark:text-gray-400 mb-8">
                    Obtenha uma cópia completa do meu currículo com detalhes sobre minha experiência e habilidades. 
                </p>
                <div class="flex flex-col md:flex-row justify-center space-x-4">
                    <Button class="mb-4 md:mb-0">
                        <Download />Baixar CV (PDF)
                    </Button>
                    <ButtonOutline>
                        <FileText />Versão DOCX
                    </ButtonOutline>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
import { Download, FileText } from 'lucide-vue-next';
import Button from '../partials/Button.vue';
import ButtonOutline from '../partials/ButtonOutline.vue';



</script>