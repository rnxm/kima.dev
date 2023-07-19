<script setup lang="ts">

    useSeoMeta({
        title: 'kima.dev | projects',
        description: 'kima\'s website thingie',
        ogTitle: 'kima.dev | projects',
        ogDescription: 'kima\'s website thingie',
        ogImage: '/favicon.png',
        ogUrl: 'https://kima.dev/projects',
        twitterTitle: 'kima.dev | projects',
        twitterDescription: 'kima\'s website thingie',
        twitterImage: '/favicon.png',
        twitterCard: 'summary'
    })

    const route = useRoute()
</script>

<template>
    <div class="bg-black h-full w-screen flex flex-col items-center justify-between p-5 font-['Roboto Slab']">
        <NavigationBar :path="route.path"/>
        <div class="h-full w-screen flex flex-col items-center justify-center select-none gap-5 my-20">
            <h1 class="text-white">here is some kind of a list of my and others projects..</h1>
            <br>
            <div class="flex flex-col gap-20 h-max w-fit">
                <div class="flex flex-col gap-10 h-fit w-fit">
                    <h1 class="text-2xl text-white font-['VT323']">own projects</h1>
                    <div class="flex flex-row flex-wrap gap-10 h-fit w-fit max-w-3xl">
                        <ProjectCard title="reFilc" description="an alternative eKréta client that looks and works better lol, made by students for students" icon_url="/images/logo/refilc.png" link="https://refilc.hu"/>
                        <ProjectCard title="Stority" description="a hungarian social media platform with many cool features and thingies" icon_url="/images/logo/stority.png" link="https://stority.hu"/>
                        <ProjectCard title="Li-Ma-Craft" description="an open minecraft server for everyone, with most known minigames like bedwars, murdermystery, etc." link="https://limacraft.kima.dev"/>
                        <ProjectCard title="Other.." description="all of my smallest and other work in progress projects are on my github page, check them out too :D" link="https://github.com/kimaah"/>
                        <!-- <ProjectCard tite="" description="" icon_url="penis" link="https://"/> -->
                    </div>
                </div>
                <div class="flex flex-col gap-10 h-fit w-fit">
                    <h1 class="text-2xl text-white font-['VT323']">projects in which i have part in</h1>
                    <div class="flex flex-row flex-wrap gap-10 h-fit w-fit max-w-3xl">
                        <ProjectCard title="Alley" description="a modern discord bot with slash commands, easy-usage and full of useful and good features" icon_url="/images/logo/alley.png" link="https://alley.hu"/>
                        <ProjectCard title="LINSE DSGN" description="a designer and partly a developer team, we are creating custom, modern and clean designs or entire websites" icon_url="/images/logo/linse.png" link="https://linse.hu"/>
                    </div>
                </div>
                <div class="flex flex-col gap-10 h-fit w-fit">
                    <h1 class="text-2xl text-white font-['VT323']">friends' projects</h1>
                    <div class="flex flex-row flex-wrap gap-10 h-fit w-fit max-w-3xl">
                        <ProjectCard title="TokyoHost" description="a game and virtual server hosting provider based in hungary with most of the popular game servers supported" icon_url="/images/logo/tokyohost.png" link="https://tokyohost.eu"/>
                        <ProjectCard title="Plave" description="another cool hungarian social media platform which is mainly based on voice and sound" icon_url="/images/logo/plave.png" link="https://plave.hu"/>
                        <ProjectCard title="FreshFM" description="a hungarian online radio station that plays new and better known older songs too" icon_url="/images/logo/freshfm.png" link="https://freshfm.hu"/>
                        <ProjectCard title="MARS" description="another designer and developer team, they're also cheap and make fancy designs" icon_url="/images/logo/mars.png" link="https://marsdesign.hu"/>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>