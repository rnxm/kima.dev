<script setup lang="ts">
	useSeoMeta({
		title: 'kima.dev | home',
		description: 'kima\'s website thingie',
		ogTitle: 'kima.dev | home',
		ogDescription: 'kima\'s website thingie',
		ogImage: '/favicon.png',
		ogUrl: 'https://kima.dev',
		twitterTitle: 'kima.dev | home',
		twitterDescription: 'kima\'s website thingie',
		twitterImage: '/favicon.png',
		twitterCard: 'summary'
	});

	const route = useRoute()
</script>

<template>
	<div class="bg-black h-screen w-screen flex flex-col items-center justify-between p-5 font-['Roboto_Slab']">
		<Navigator :path="route.path"/>
		<div class="h-screen w-screen flex flex-col items-center justify-center select-none gap-5">
			<h1 class="text-white">kima.dev</h1>
		</div>
	</div>
</template>
