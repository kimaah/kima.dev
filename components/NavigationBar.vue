<script setup lang="ts">
    defineProps({
        path: {
            type: String,
            default: '/'
        }
    })
</script>

<template>
    <div class="flex flex-row flex-wrap items-center justify-center gap-5 select-none font-['VT323'] text-[21px] fixed top-0 left-0 right-0 backdrop-blur-[6px] bg-[#00000044] border-b border-[#00000044] z-50 py-4 px-3">
        <NuxtLink to="/">
            <h1 class="hover:underline" :class="path == '/' ? 'text-violet-300' : 'text-white'">home</h1>
        </NuxtLink>
        <p class="text-white">•</p>
        <NuxtLink to="/about">
            <p class="hover:underline" :class="path == '/about' ? 'text-violet-300' : 'text-white'">about</p>
        </NuxtLink>
        <p class="text-white">•</p>
        <NuxtLink to="/projects">
            <p class="hover:underline" :class="path == '/projects' ? 'text-violet-300' : 'text-white'">projects</p>
        </NuxtLink>
        <p class="text-white">•</p>
        <NuxtLink to="/contact">
            <p class="hover:underline" :class="path == '/contact' ? 'text-violet-300' : 'text-white'">contact</p>
        </NuxtLink>
        <p class="text-white">•</p>
        <NuxtLink to="/something">
            <p class="hover:underline" :class="path == '/something' ? 'text-red-500' : 'text-white'">something :3</p>
        </NuxtLink>
    </div>
</template>