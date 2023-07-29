<script setup lang="ts">
    const route = useRoute()
</script>

<template>
    <div class="bg-black h-full w-full flex flex-col items-center justify-between p-5 font-['Georgia']">
        <NavigationBar :path="route.path" />
        <NuxtPage />
    </div>
</template>