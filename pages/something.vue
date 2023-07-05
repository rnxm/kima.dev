<script setup lang="ts">
    useSeoMeta({
        title: 'kima.dev | something',
        description: 'kima\'s website thingie',
        ogTitle: 'kima.dev | something',
        ogDescription: 'kima\'s website thingie',
        ogImage: '/favicon.ico',
        ogUrl: 'https://kima.dev/something',
        twitterTitle: 'kima.dev | something',
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
            <h1 class="text-white text-center"><span class="text-red-500">a</span>ctu<span class="text-red-500">all</span>y <span class="text-red-500">n</span>oth<span class="text-red-500">in</span>g spec<span class="text-red-500">ia</span>l, but...<br>...<span class="text-red-500">i</span> <span class="text-red-500">l</span>ove my g<span class="text-red-500">i</span>r<span class="text-red-500">l</span>fr<span class="text-red-500">i</span>e<span class="text-red-500">nd</span> SO MUCH! <span class="text-red-500">&lt;3</span></h1>
        </div>
    </div>
</template>
