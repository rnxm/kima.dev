<script setup lang="ts">
    useSeoMeta({
        title: 'kima.dev | about',
        description: 'kima\'s website thingie',
        ogTitle: 'kima.dev | about',
        ogDescription: 'kima\'s website thingie',
        ogImage: '/favicon.png',
        ogUrl: 'https://kima.dev/about',
        twitterTitle: 'kima.dev | about',
        twitterDescription: 'kima\'s website thingie',
        twitterImage: '/favicon.png',
        twitterCard: 'summary'
    })
</script>

<template>
    <div class="h-full w-fit flex flex-col items-start justify-center select-none gap-5 text-white">
        <p class="text-justify indent-[-1em] ml-4">
            • hi! i'm kima, a full-stack web developer :3
        </p>
        <p class="text-justify indent-[-1em] ml-4">
            • i use things like python, html, css, javascript, some web frameworks like nuxt, etc.<br>
            ohh actually i love flutter mobile framework too..<br>
            visual studio code forever :hot_face:<br>
            fuck php and other shit langs like that
        </p>
        <p class="text-justify indent-[-1em] ml-4">
            • i'm from hungary<br>
            currently i'm 15 years old :rolling_eyes:<br>
            i live in szigetszentmiklós
        </p>
        <p class="text-justify indent-[-1em] ml-4">
            • another fun fact about me <span class="italic hover:underline"><NuxtLink to="/something">here</NuxtLink></span>
        </p>
    </div>
</template>
