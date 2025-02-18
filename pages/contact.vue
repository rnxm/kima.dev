<script setup lang="ts">
    useSeoMeta({
        title: 'kima.dev | contact',
        description: 'kima\'s website thingie',
        ogTitle: 'kima.dev | contact',
        ogDescription: 'kima\'s website thingie',
        ogImage: '/favicon.png',
        ogUrl: 'https://kima.dev/contact',
        twitterTitle: 'kima.dev | contact',
        twitterDescription: 'kima\'s website thingie',
        twitterImage: '/favicon.png',
        twitterCard: 'summary'
    })
</script>

<template>
    <div class="h-full w-full flex flex-col items-center justify-center select-none gap-5">
        <div class="h-max w-max flex flex-row flex-wrap text-white gap-10">
            <a href="https://t.me/kimaaah" target="_blank" class="transition ease-in-out hover:opacity-75 duration-200">
                <Icon name="fa6-brands:telegram" size="32px" />
            </a>
            <a href="https://discord.com/users/654721418273226793" target="_blank" class="transition ease-in-out hover:opacity-75 duration-200">
                <Icon name="fa6-brands:discord" size="32px" />
            </a>
            <a href="https://instagr.am/k1m4h_" target="_blank" class="transition ease-in-out hover:opacity-75 duration-200">
                <Icon name="fa6-brands:instagram" size="32px" />
            </a>
            <a href="https://github.com/kimaah" target="_blank" class="transition ease-in-out hover:opacity-75 duration-200">
                <Icon name="fa6-brands:github" size="32px" />
            </a>
            <a href="https://yoursit.ee/kima" target="_blank" class="transition ease-in-out hover:opacity-75 duration-200">
                <Icon name="fa6-solid:ellipsis" size="32px" />
            </a>
        </div>
    </div>
</template>
