<script setup lang="ts">
    const route = useRoute()
</script>

<template>
    <div class="bg-black w-full flex flex-col items-center justify-between p-5 font-['Georgia']" :class="route.path == '/projects' ? 'h-full' : 'h-screen'">
        <NavigationBar :path="route.path" />
        <NuxtPage />
    </div>
</template>