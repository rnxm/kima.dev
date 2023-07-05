<script setup lang="ts">
    useSeoMeta({
        title: 'kima.dev | projects',
        description: 'kima\'s website thingie',
        ogTitle: 'kima.dev | projects',
        ogDescription: 'kima\'s website thingie',
        ogImage: '/favicon.ico',
        ogUrl: 'https://kima.dev/projects',
        twitterTitle: 'kima.dev | projects',
        twitterDescription: 'kima\'s website thingie',
        twitterImage: '/favicon.ico',
        twitterCard: 'summary'
    });
    useHead({
        htmlAttrs: {
            lang: 'en'
        },
        link: [
            {
                rel: 'icon',
                type: 'image/png',
                href: '/favicon.png'
            }
        ]
    });

    const route = useRoute();
</script>

<template>
    <div class="bg-black h-screen w-screen flex flex-col items-center justify-between p-5">
        <Navigator :path="route.path"/>
        <div class="h-screen w-screen flex flex-col items-center justify-center select-none gap-5">
            <h1 class="text-white">omg a lot, i will list them here soon..</h1>
        </div>
    </div>
</template>