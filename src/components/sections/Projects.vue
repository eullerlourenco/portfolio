<template>
    <section class="py-12 md:py-14 bg-linear-to-br from-gray-900/75 to-gray-900" id="projects">
        <div class="container mx-auto px-4 flex flex-col items-center justify-center">
            <h1 class="text-4xl font-bold my-4 mb-12">
                    <span class="font-normal text-violet-900 font-mono"><</span> 
                    Meus Projetos
                    <span class="font-normal text-violet-900 font-monp">/></span>
                </h1>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <div v-for="project in projects" :key="project.title"
                    class="rounded-lg overflow-hidden border border-gray-200 dark:border-gray-800 bg-white dark:bg-gray-950 shadow-sm hover:shadow-md transition-shadow"> 
                    <div class="h-48 bg-gray-200 dark:bg-gray-800">
                        <img :src="project.image" :alt="`Imagem do ${project.title}`"
                            class="w-full h-full object-cover" />
                    </div>
                    <div class="p-6">
                        <h3 class="text-xl font-semibold text-gray-900 dark:text-white mb-2">{{ project.title }}</h3>
                        <p class="text-gray-600 dark:text-gray-300 mb-4">
                            Uma breve descrição do projeto, destacando as principais características e tecnologias
                            utilizadas.
                        </p>
                        <div class="flex flex-wrap gap-2 mb-4">
                            <span v-for="habilite in project.habilites" :key="habilite"
                                class="px-3 py-1 text-xs rounded-full bg-linear-to-br dark:from-gray-800 dark:to-gray-900/35 text-gray-800 dark:text-gray-300">
                                {{ habilite }}
                            </span>
                        </div>
                        <div class="flex self-end justify-end space-x-3">
                            <a :href="project.link" target="_blank"
                                class="border-1 dark:border-gray-600 hover-violet-shadow hover:text-violet-700 hover:border-violet-700 rounded-full p-2.5 text-gray-500 text-gray-600">
                                <Github class="h-5 w-5" />
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script setup>
import { ExternalLink, Github } from 'lucide-vue-next';


const projects = [
    {
        title: 'Líder Gás - ERP',
        description: 'Sistema ERP para gestão de vendas, estoque e financeiro de uma revendedora de gás.',
        image: 'https://placehold.co/384x192/000/f1f1f1',
        link: '#',
        habilites: ['CodeIgniter 4', 'Bootstrap', 'JavaScript']
    },
    {
        title: 'LSTasks - Gerenciador de Tarefas',
        description: 'Gerenciador de tarefas, onde o usuário pode adicionar, editar e remover tarefas. Com autenticação e autorização de usuários.',
        image: 'https://placehold.co/300/000/f1f1f1',
        link: '#',
        habilites: ['Laravel', 'Tailwind CSS', 'JavaScript']
    },
    {
        title: 'Todo List - Lista de Tarefas',  
        description: 'Uma lista de tarefas simples, onde o usuário pode adicionar, editar e remover tarefas.',
        image: 'https://placehold.co/300/000/f1f1f1',
        link: '#',
        habilites: ['CodeIgniter 4', 'Bootstrap']
    }
];

</script>