<script setup lang="ts">
    const props = defineProps({
        title: {
            type: String,
            default: '???'
        },
        description: {
            type: String,
            default: 'Nincs leírás megadva..'
        },
        icon_url: {
            type: String,
            default: '/images/placeholder.png'
        },
        link: {
            type: String,
            default: '#'
        }
    })

    var img_b_class = ''
    if (props.icon_url == '/images/placeholder.png') {
        img_b_class = 'border border-white'
    }
</script>

<template>
    <a :href="link" target="_blank" class="transition ease-in-out hover:scale-[1.03] duration-200">
        <div class="flex flex-row items-start justify-center gap-5 select-none">
            <div class="h-fit w-fit">
                <div class="rounded-full w-12 h-12 border border-white absolute z-10"></div>
                <img :src="icon_url" alt="logo" class="rounded-full w-12 h-12 ml-2 mt-2" :class="img_b_class">
            </div>
            <div class="flex flex-col items-start justify-center gap-2">
                <h1 class="text-[23px] font-medium text-white font-['VT323'] leading-3">{{ title }}</h1>
                <p class="text-[15px] text-white max-w-[250px]">{{ description }}</p>
            </div>
        </div>
    </a>
</template>