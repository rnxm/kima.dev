<script setup lang="ts">
    const props = defineProps({
        error: Object
    })
    const handleError = () => clearError({ redirect: '/' })

    const route = useRoute()

    useSeoMeta({
        title: `kima.dev | ${props.error?.statusCode}`,
        description: 'kima\'s website thingie',
        ogTitle: `kima.dev | ${props.error?.statusCode}`,
        ogDescription: 'kima\'s website thingie',
        ogImage: '/favicon.png',
        ogUrl: `https://kima.dev${route.path}`,
        twitterTitle: `kima.dev | ${props.error?.statusCode}`,
        twitterDescription: 'kima\'s website thingie',
        twitterImage: '/favicon.png',
        twitterCard: 'summary'
    })
</script>

<template>
	<div class="bg-black h-screen w-screen flex flex-col items-center justify-between p-5 font-['Roboto_Slab']">
		<NavigationBar path="?"/>
		<div class="h-screen w-screen flex flex-col items-center justify-center select-none gap-5">
			<h1 class="text-white text-center">
                {{ error?.statusCode }} - {{ error?.statusMessage.toLowerCase() }}<br>
                click <span @click="handleError" class="italic hover:underline cursor-pointer">here</span> to go to home page
            </h1>
		</div>
	</div>
</template>