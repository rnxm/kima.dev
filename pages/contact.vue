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

    const route = useRoute()
</script>

<template>
    <div class="bg-black h-screen w-screen flex flex-col items-center justify-between p-5 font-['Roboto Slab']">
        <NavigationBar :path="route.path"/>
        <div class="h-screen w-screen flex flex-col items-center justify-center select-none gap-5">
            <div class="h-max w-max flex flex-row flex-wrap text-white gap-10">
                <a href="https://t.me/kimaaah" target="_blank" class="transition ease-in-out hover:opacity-75 duration-200">
                    <Icon name="fa6-brands:telegram" size="32px" />
                </a>
                <a href="https://discord.com/channels/@me/654721418273226793" target="_blank" class="transition ease-in-out hover:opacity-75 duration-200">
                    <Icon name="fa6-brands:discord" size="32px" />
                </a>
                <a href="https://instagr.am/__k1m4__" target="_blank" class="transition ease-in-out hover:opacity-75 duration-200">
                    <Icon name="fa6-brands:instagram" size="32px" />
                </a>
                <a href="https://github.com/kimaah" target="_blank" class="transition ease-in-out hover:opacity-75 duration-200">
                    <Icon name="fa6-brands:github" size="32px" />
                </a>
                <a href="https://xyl.lol/kima" target="_blank" class="transition ease-in-out hover:opacity-75 duration-200">
                    <Icon name="fa6-solid:ellipsis" size="32px" />
                </a>
            </div>
        </div>
    </div>
</template>
